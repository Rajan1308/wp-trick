# wp-trick

`
function num_db_queries() {
	global $wpdb;
	// if(is_developer()){
		echo  get_num_queries();
		echo ' queries in ';
		timer_stop( );
		echo 'second';

		echo "<pre>";print_r($wpdb->queries); echo "</pre>";
	// }
}
add_action('wp_footer', 'num_db_queries');

`
