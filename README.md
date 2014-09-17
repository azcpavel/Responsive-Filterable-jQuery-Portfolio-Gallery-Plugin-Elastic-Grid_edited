Responsive-Filterable-jQuery-Portfolio-Gallery-Plugin-Elastic-Grid_edited
=========================================================================

Loading html instead of image with random fx


Just use elastic_grid_edited.js & load with this function

Note: try to keep yout thumb img height to 100px


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
