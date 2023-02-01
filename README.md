# assignment2-lingam
To learn more about markdown

# Joyce Lingam
I love Cricket especially **Indian** Cricket Team, they always makes us proud in World cup Finials.
They will be 15 players in this game and the caption of the cricket is **Mr.Virat Kohli**.
____
# Team India 

1. M.S Dhoni
2. Virat Kholi 
3. Bravo
_____
# Other Teams

* England  
* Austrila 
* Pakstian 
_____

![click here to know about me](https://github.com/JoyceLingam/assignment2-lingam/blob/main/AboutMe.md) T

___
# To create a table with 4 countries

This table contains my favorite countries to travel

|**Countries**|**Where to go**|**Number of days**|
|-------------|----------------|----------------|
|Spain|Visit Prado Museum|2 days|
|Russia|Visit Huge Siberian Lake|3 days|
|United States|Visit Newyork|5 days|
|France|Visit Eiffel|6 days|

____
# Funny Quotes
1. `"people who live in the glass house have to answer the door"` --- by **_karl pilkington_**
2. `"There is nothing better than a friend, Unless it's a friend with chocolate."` --- by **_Linda Grayson_**

____
### CODE FENCING 
 
 [link to question] (https://www.javatpoint.com/jquery-interview-questions)
 
 ```

 (function($) {
    $.fn.drags = function(opt) {

        opt = $.extend({handle:"",cursor:"move"}, opt);

        if(opt.handle === "") {
            var $el = this;
        } else {
            var $el = this.find(opt.handle);
        }

        return $el.css('cursor', opt.cursor).on("mousedown", function(e) {
            if(opt.handle === "") {
                var $drag = $(this).addClass('draggable');
            } else {
                var $drag = $(this).addClass('active-handle').parent().addClass('draggable');
            }
            var z_idx = $drag.css('z-index'),
                drg_h = $drag.outerHeight(),
                drg_w = $drag.outerWidth(),
                pos_y = $drag.offset().top + drg_h - e.pageY,
                pos_x = $drag.offset().left + drg_w - e.pageX;
            $drag.css('z-index', 1000).parents().on("mousemove", function(e) {
                $('.draggable').offset({
                    top:e.pageY + pos_y - drg_h,
                    left:e.pageX + pos_x - drg_w
                }).on("mouseup", function() {
                    $(this).removeClass('draggable').css('z-index', z_idx);
                });
            });
            e.preventDefault(); // disable selection
        }).on("mouseup", function() {
            if(opt.handle === "") {
                $(this).removeClass('draggable');
            } else {
                $(this).removeClass('active-handle').parent().removeClass('draggable');
            }
        });

    }
})(jQuery);

```
[Link for Reference Source URL] (https://css-tricks.com/snippets/jquery/draggable-without-jquery-ui/)


