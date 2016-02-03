# WP-REST-API-jQuery

jQuery SDK for [WordPress REST API](https://github.com/WP-API/WP-API).


## Usage
```javascrript
         jQuery(function($){
             $('#login').on('click',function(e){
                e.preventDefault();
                $(this).wpBasicAuth({

                        url:'http://resttest.com/wp-json/wp/v2/posts/4',
                        method: $('#action').val(),
                        /*
                        username and password.
                        */
                        /*               
                        username:'suifengtec',
                        password:'coolwp!r$',
                        */
                        /*
                        or give it the selectors of the username and the password.
                        */
                        username_c:'#name',
                        password_c:'#pswd',
                        callback: function(status,data){

                            window.console.log( 'status' );
                            window.console.log( status );
                            window.console.log( 'data' );
                            window.console.log( data );

                        }
                });
             });
         });

```

## TEST

![ GET ](https://raw.githubusercontent.com/CoolWP/WP-REST-API-jQuery/master/screenshot-1.jpg)
![ a wrong user DELETE a post ](https://raw.githubusercontent.com/CoolWP/WP-REST-API-jQuery/master/screenshot-2.jpg)
![ a right user DELETE a post ](https://raw.githubusercontent.com/CoolWP/WP-REST-API-jQuery/master/screenshot-3.jpg)
