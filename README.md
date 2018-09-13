<!--
author:   Andre Dietrich
email:    your@email.com
version:  0.1.0
language: en
narrator: US English Female

comment:  This simple description of your course.
          Multiline is also okay.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

translation: Français translations/French.md


link:  https://pannellum.org/css/style.css
       https://cdn.pannellum.org/2.4/pannellum.css

script: https://cdn.pannellum.org/2.4/pannellum.js

@panorama
<div id="panorama_@0" style="width: 100%; height: 400px;"></div>

<script>
  pannellum.viewer('panorama_@0', {
        "type": "equirectangular",
        "panorama": "@1",
        "autoLoad": true,
        "hotSpots": [@2]
  });
</script>
@end


-->

# MeetupDemo

Just a simple LiaScript demo course, see the rendered version at:

https://liascript.github.io/course/?https://raw.githubusercontent.com/andre-dietrich/MeetupDemo/master/README.md

**Github project:**

https://github.com/andre-dietrich/MeetupDemo

**Further Usefull links:**

* The project: http://LiaScript.github.io
* Atom plugins:
  * Previewer:  https://atom.io/packages/liascript-preview
  * Snippets & help:  https://atom.io/packages/liascript-snippets


## The eLab (Pre-History)

<iframe width="100%" height="500px" src="https://www.youtube.com/embed/bICfKRyKTwE" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


## Multimedia

![image](https://cdn-images-1.medium.com/max/1600/1*eefaDiYhxtm3QdokHb-Nqg.jpeg)<!-- width="100%" -->


?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)


!?[movie](https://www.youtube.com/embed/bICfKRyKTwE)


## Effects and TTS


      --{{1 French Female}}--
At first there is a table.


     {{1}}
| Header 1   | Header 2   | Header 3   | Header 4   | Header 5   | Header 6   |
| :--------- | :--------- | :--------- | :--------- | :--------- | :--------- |
| Item 1     | Item 2     | Item 3     | Item 4     | Item 5     | Item 6     |

    --{{2}}--
Then comes a list.


    {{2-3}}
* list
* xxx

    --{{3}}--
And then comes something else.


     {{3}}
This is an *ordinary* paragraph.


## ASCII-Art

               Title - dots
6 | A a B b C c
  | D d E e F f G g H h I i
  | J j K k L l M m N n o O
  | P p Q q R r S s T t U u
  | V v W w X x Y y Z Z   *
1 +------------------------
  0                      24


                                Multiline
1.9 |
    |                 ***
  y |               *     *        r
  - | r r r r r r r*r r r r*r r r
  a |             *         *     K
  x |            *           *   KKK
  i | B B B B B * B B B B B B * B B B B B
  s |         *                 *
    | *  * *                       * *  *
 -1 +------------------------------------
    0              x-axis               10

## Quizzes


   [[solution]]
   <script>
     // @input will be replace by the user input
     let input_string = @input;
     "solution" == input_string.trim().toLowerCase();
   </script>


   [( )] This is wrong.
   [(X)] The only correct option.
   [( )] Still not right.
   [( )] Still not right.
   [[?]] hint
   [[?]] hint2
   ****************************************

   Add a solution explanation __Markdown__!

   ****************************************

   [[ ]] Add as many elements as you want?
   [[X]] The X marks the correct answer!
   [[ ]] ... this is wrong ...
   [[X]] ... this has to be selected too ...

## Surveys

[(:bad)(:not good)(:good)]
[         ] text
[         ] text
[         ] text

## Programming


``` js     -EvalScript.js
let who = data.first_name + " " + data.last_name;

if(data.online) {
  who + " is online"; }
else {
  who + " is NOT online"; }
```
``` json    +Data.json
{
  "first_name" :  "Sammy",
  "last_name"  :  "Shark",
  "online"     :  true
}
```
<script>
  // insert the JSON dataset into the local variable data
  let data = @input(1);

  // eval the script that uses this dataset
  eval(`@input(0)`);
</script>


## Extensions & Macros


@panorama(1,https://pannellum.org/images/cerro-toco-0.jpg,{})


```json
@panorama(0,https://pannellum.org/images/bma-1.jpg)

{
    "pitch": 14.1,
    "yaw": 1.5,
    "type": "info",
    "text": "Baltimore Museum of Art",
    "URL": "https://artbma.org/"
},
{
    "pitch": -9.4,
    "yaw": 222.6,
    "type": "info",
    "text": "Art Museum Drive"
},
{
    "pitch": -0.9,
    "yaw": 144.4,
    "type": "info",
    "text": "North Charles Street"
}
```
