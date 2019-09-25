public function remove_admin_menu_bar_items ($wp_toolbar) {
    $wp_toolbar->remove_node( 'my-sites' );
    $wp_toolbar->remove_node( 'wp-logo' );
    $wp_toolbar->remove_node( 'new-content' );
    $wp_toolbar->remove_node( 'view' );
    $wp_toolbar->remove_node( 'search' );  // remove the search element
    return $wp_toolbar;
}
add_filter( 'admin_bar_menu', 'remove_admin_menu_bar_items' );
