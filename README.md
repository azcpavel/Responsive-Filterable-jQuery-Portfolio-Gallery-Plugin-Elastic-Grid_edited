Responsive-Filterable-jQuery-Portfolio-Gallery-Plugin-Elastic-Grid_edited
=========================================================================

Loading html instead of image with random fx
enable navigation
added after onclick options

Just use elastic_grid_edited.js & load with this function

Note: try to keep your thumb img height to 100px

<script src="js/jquery.hoverdir.js"></script>
<script src="js/jquery.elastislide.js"> </script>


```
$(function(){
        var fxrand = Math.floor((Math.random() * 5) + 1);
        var fx = ['fallperspective', 'fly', 'flip', 'helix' , 'popup'];
        $("#elastic_grid").elastic_grid({
            'filterEffect': fx[fxrand], // moveup, scaleup, fallperspective, fly, flip, helix , popup
            'hoverDirection': true,
            'hoverDelay': 0,
            'hoverInverse': false,
            'expandingSpeed': 500,
            'expandingHeight': 570,
            exHideInfoBoxTitle: false, // Added New Variable For Hiding Title in infobox 
            exControls: false, // Added new variable for control flag
            exControlsCSS : {position:'absolute', cursor:'pointer', padding : 5, marginTop : '15%'}, // Added new variable for control css
            exControlsNextText : 'Next', // Added new variable for control next text
            exControlsNextClass : null, // Added new variable for control next class
            exControlsPrevText : 'Prev', // Added new variable for control prev text
            exControlsPrevClass : null, // Added new variable for control prev class
            exOnClickEvent: function() { console.log('Test')}, // Added New Variable For After Click Action
            'items' :
            [
                {
                    'title'         : 'Simple Accounting',
                    'description'   : 'Accounting System<br> * Development Tool: PHP5, Codeigniter, jQuery <br>* Transaction Management<br>* Asset management<br>* User Management<br>* E-Payment Management<br>* Dropdown Management<br>Username: admin<br>Password: 1234',
                    'thumbnail'     : ['http://www.itszahid.info/images/acc/thumb/1.jpg', 'http://www.itszahid.info/images/acc/thumb/2.jpg'],
                    'large'         : ['<img src="http://www.itszahid.info/images/acc/1.png"/>', '<img src="http://www.itszahid.info/images/acc/2.png"/>'],
                    'button_list'   :
                    [
                        { 'title':'Demo', 'url' : 'http://www.exceptionsolutions.info/projects/account' }                        
                    ],
                    'tags'          : ['Web Application']                    
                }
            ]
        });
});

```
