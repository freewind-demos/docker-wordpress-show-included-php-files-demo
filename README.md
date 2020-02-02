Docker Wordpress Show Included Php Files Demo
=============================================

通过`get_included_files`这个函数，得到所有被include的文件。


```
npm run up
```

在首页的源代码最后，可以看到很多文件名：

```
/var/www/html/index.php
/var/www/html/wp-blog-header.php
/var/www/html/wp-load.php
/var/www/html/wp-config.php
/var/www/html/wp-settings.php
/var/www/html/wp-includes/version.php
/var/www/html/wp-includes/load.php
/var/www/html/wp-includes/class-wp-paused-extensions-storage.php
/var/www/html/wp-includes/class-wp-fatal-error-handler.php
/var/www/html/wp-includes/class-wp-recovery-mode-cookie-service.php
/var/www/html/wp-includes/class-wp-recovery-mode-key-service.php
/var/www/html/wp-includes/class-wp-recovery-mode-link-service.php
/var/www/html/wp-includes/class-wp-recovery-mode-email-service.php
/var/www/html/wp-includes/class-wp-recovery-mode.php
/var/www/html/wp-includes/error-protection.php
/var/www/html/wp-includes/default-constants.php
/var/www/html/wp-includes/plugin.php
/var/www/html/wp-includes/class-wp-hook.php
/var/www/html/wp-includes/compat.php
/var/www/html/wp-includes/class-wp-list-util.php
/var/www/html/wp-includes/formatting.php
/var/www/html/wp-includes/meta.php
/var/www/html/wp-includes/functions.php
/var/www/html/wp-includes/option.php
/var/www/html/wp-includes/class-wp-meta-query.php
/var/www/html/wp-includes/class-wp-matchesmapregex.php
/var/www/html/wp-includes/class-wp.php
/var/www/html/wp-includes/class-wp-error.php
/var/www/html/wp-includes/pomo/mo.php
/var/www/html/wp-includes/pomo/translations.php
/var/www/html/wp-includes/pomo/plural-forms.php
/var/www/html/wp-includes/pomo/entry.php
/var/www/html/wp-includes/pomo/streams.php
/var/www/html/wp-includes/wp-db.php
/var/www/html/wp-includes/cache.php
/var/www/html/wp-includes/default-filters.php
/var/www/html/wp-includes/l10n.php
/var/www/html/wp-includes/class-wp-locale.php
/var/www/html/wp-includes/class-wp-locale-switcher.php
/var/www/html/wp-includes/class-wp-walker.php
/var/www/html/wp-includes/class-wp-ajax-response.php
/var/www/html/wp-includes/capabilities.php
/var/www/html/wp-includes/class-wp-roles.php
/var/www/html/wp-includes/class-wp-role.php
/var/www/html/wp-includes/class-wp-user.php
/var/www/html/wp-includes/class-wp-query.php
/var/www/html/wp-includes/query.php
/var/www/html/wp-includes/class-wp-date-query.php
/var/www/html/wp-includes/theme.php
/var/www/html/wp-includes/class-wp-theme.php
/var/www/html/wp-includes/template.php
/var/www/html/wp-includes/class-wp-user-request.php
/var/www/html/wp-includes/user.php
/var/www/html/wp-includes/class-wp-user-query.php
/var/www/html/wp-includes/class-wp-session-tokens.php
/var/www/html/wp-includes/class-wp-user-meta-session-tokens.php
/var/www/html/wp-includes/class-wp-metadata-lazyloader.php
/var/www/html/wp-includes/general-template.php
/var/www/html/wp-includes/link-template.php
/var/www/html/wp-includes/author-template.php
/var/www/html/wp-includes/post.php
/var/www/html/wp-includes/class-walker-page.php
/var/www/html/wp-includes/class-walker-page-dropdown.php
/var/www/html/wp-includes/class-wp-post-type.php
/var/www/html/wp-includes/class-wp-post.php
/var/www/html/wp-includes/post-template.php
/var/www/html/wp-includes/revision.php
/var/www/html/wp-includes/post-formats.php
/var/www/html/wp-includes/post-thumbnail-template.php
/var/www/html/wp-includes/category.php
/var/www/html/wp-includes/class-walker-category.php
/var/www/html/wp-includes/class-walker-category-dropdown.php
/var/www/html/wp-includes/category-template.php
/var/www/html/wp-includes/comment.php
/var/www/html/wp-includes/class-wp-comment.php
/var/www/html/wp-includes/class-wp-comment-query.php
/var/www/html/wp-includes/class-walker-comment.php
/var/www/html/wp-includes/comment-template.php
/var/www/html/wp-includes/rewrite.php
/var/www/html/wp-includes/class-wp-rewrite.php
/var/www/html/wp-includes/feed.php
/var/www/html/wp-includes/bookmark.php
/var/www/html/wp-includes/bookmark-template.php
/var/www/html/wp-includes/kses.php
/var/www/html/wp-includes/cron.php
/var/www/html/wp-includes/deprecated.php
/var/www/html/wp-includes/script-loader.php
/var/www/html/wp-includes/class-wp-dependency.php
/var/www/html/wp-includes/class.wp-dependencies.php
/var/www/html/wp-includes/class.wp-scripts.php
/var/www/html/wp-includes/functions.wp-scripts.php
/var/www/html/wp-includes/class.wp-styles.php
/var/www/html/wp-includes/functions.wp-styles.php
/var/www/html/wp-includes/taxonomy.php
/var/www/html/wp-includes/class-wp-taxonomy.php
/var/www/html/wp-includes/class-wp-term.php
/var/www/html/wp-includes/class-wp-term-query.php
/var/www/html/wp-includes/class-wp-tax-query.php
/var/www/html/wp-includes/update.php
/var/www/html/wp-includes/canonical.php
/var/www/html/wp-includes/shortcodes.php
/var/www/html/wp-includes/embed.php
/var/www/html/wp-includes/class-wp-embed.php
/var/www/html/wp-includes/class-wp-oembed.php
/var/www/html/wp-includes/class-wp-oembed-controller.php
/var/www/html/wp-includes/media.php
/var/www/html/wp-includes/http.php
/var/www/html/wp-includes/class-http.php
/var/www/html/wp-includes/class-requests.php
/var/www/html/wp-includes/class-wp-http-streams.php
/var/www/html/wp-includes/class-wp-http-curl.php
/var/www/html/wp-includes/class-wp-http-proxy.php
/var/www/html/wp-includes/class-wp-http-cookie.php
/var/www/html/wp-includes/class-wp-http-encoding.php
/var/www/html/wp-includes/class-wp-http-response.php
/var/www/html/wp-includes/class-wp-http-requests-response.php
/var/www/html/wp-includes/class-wp-http-requests-hooks.php
/var/www/html/wp-includes/Requests/Hooks.php
/var/www/html/wp-includes/Requests/Hooker.php
/var/www/html/wp-includes/widgets.php
/var/www/html/wp-includes/class-wp-widget.php
/var/www/html/wp-includes/class-wp-widget-factory.php
/var/www/html/wp-includes/nav-menu.php
/var/www/html/wp-includes/nav-menu-template.php
/var/www/html/wp-includes/class-walker-nav-menu.php
/var/www/html/wp-includes/admin-bar.php
/var/www/html/wp-includes/rest-api.php
/var/www/html/wp-includes/rest-api/class-wp-rest-server.php
/var/www/html/wp-includes/rest-api/class-wp-rest-response.php
/var/www/html/wp-includes/rest-api/class-wp-rest-request.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-posts-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-attachments-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-post-types-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-post-statuses-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-revisions-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-autosaves-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-taxonomies-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-terms-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-users-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-comments-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-search-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-blocks-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-block-renderer-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-settings-controller.php
/var/www/html/wp-includes/rest-api/endpoints/class-wp-rest-themes-controller.php
/var/www/html/wp-includes/rest-api/fields/class-wp-rest-meta-fields.php
/var/www/html/wp-includes/rest-api/fields/class-wp-rest-comment-meta-fields.php
/var/www/html/wp-includes/rest-api/fields/class-wp-rest-post-meta-fields.php
/var/www/html/wp-includes/rest-api/fields/class-wp-rest-term-meta-fields.php
/var/www/html/wp-includes/rest-api/fields/class-wp-rest-user-meta-fields.php
/var/www/html/wp-includes/rest-api/search/class-wp-rest-search-handler.php
/var/www/html/wp-includes/rest-api/search/class-wp-rest-post-search-handler.php
/var/www/html/wp-includes/class-wp-block-type.php
/var/www/html/wp-includes/class-wp-block-styles-registry.php
/var/www/html/wp-includes/class-wp-block-type-registry.php
/var/www/html/wp-includes/class-wp-block-parser.php
/var/www/html/wp-includes/blocks.php
/var/www/html/wp-includes/blocks/archives.php
/var/www/html/wp-includes/blocks/block.php
/var/www/html/wp-includes/blocks/calendar.php
/var/www/html/wp-includes/blocks/categories.php
/var/www/html/wp-includes/blocks/latest-comments.php
/var/www/html/wp-includes/blocks/latest-posts.php
/var/www/html/wp-includes/blocks/rss.php
/var/www/html/wp-includes/blocks/search.php
/var/www/html/wp-includes/blocks/shortcode.php
/var/www/html/wp-includes/blocks/tag-cloud.php
/var/www/html/wp-includes/vars.php
/var/www/html/wp-includes/pluggable.php
/var/www/html/wp-includes/pluggable-deprecated.php
/var/www/html/wp-includes/default-widgets.php
/var/www/html/wp-includes/widgets/class-wp-widget-pages.php
/var/www/html/wp-includes/widgets/class-wp-widget-links.php
/var/www/html/wp-includes/widgets/class-wp-widget-search.php
/var/www/html/wp-includes/widgets/class-wp-widget-archives.php
/var/www/html/wp-includes/widgets/class-wp-widget-media.php
/var/www/html/wp-includes/widgets/class-wp-widget-media-audio.php
/var/www/html/wp-includes/widgets/class-wp-widget-media-image.php
/var/www/html/wp-includes/widgets/class-wp-widget-media-video.php
/var/www/html/wp-includes/widgets/class-wp-widget-media-gallery.php
/var/www/html/wp-includes/widgets/class-wp-widget-meta.php
/var/www/html/wp-includes/widgets/class-wp-widget-calendar.php
/var/www/html/wp-includes/widgets/class-wp-widget-text.php
/var/www/html/wp-includes/widgets/class-wp-widget-categories.php
/var/www/html/wp-includes/widgets/class-wp-widget-recent-posts.php
/var/www/html/wp-includes/widgets/class-wp-widget-recent-comments.php
/var/www/html/wp-includes/widgets/class-wp-widget-rss.php
/var/www/html/wp-includes/widgets/class-wp-widget-tag-cloud.php
/var/www/html/wp-includes/widgets/class-wp-nav-menu-widget.php
/var/www/html/wp-includes/widgets/class-wp-widget-custom-html.php
/var/www/html/wp-content/themes/twentytwenty/functions.php
/var/www/html/wp-content/themes/twentytwenty/inc/template-tags.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-svg-icons.php
/var/www/html/wp-content/themes/twentytwenty/inc/svg-icons.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-customize.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-separator-control.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-walker-comment.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-walker-page.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-script-loader.php
/var/www/html/wp-content/themes/twentytwenty/classes/class-twentytwenty-non-latin-languages.php
/var/www/html/wp-content/themes/twentytwenty/inc/custom-css.php
/var/www/html/wp-includes/Requests/Cookie/Jar.php
/var/www/html/wp-includes/Requests/IRI.php
/var/www/html/wp-includes/Requests/IDNAEncoder.php
/var/www/html/wp-includes/Requests/Transport/cURL.php
/var/www/html/wp-includes/Requests/Transport.php
/var/www/html/wp-includes/Requests/Response.php
/var/www/html/wp-includes/Requests/Response/Headers.php
/var/www/html/wp-includes/Requests/Utility/CaseInsensitiveDictionary.php
/var/www/html/wp-includes/template-loader.php
/var/www/html/wp-content/themes/twentytwenty/index.php
/var/www/html/wp-content/themes/twentytwenty/header.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/modal-search.php
/var/www/html/wp-content/themes/twentytwenty/searchform.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/modal-menu.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/content.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/entry-header.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/featured-image.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/pagination.php
/var/www/html/wp-content/themes/twentytwenty/template-parts/footer-menus-widgets.php
/var/www/html/wp-content/themes/twentytwenty/footer.php
```
