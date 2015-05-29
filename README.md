#Material Color

Material Color is a javascript color generator. It is helpful when creating designs that follow Google Material Design.

##Usage

###Node:
    var MaterialColor = require('MaterialColor');

###Browser:
    <script src="color.js"></script>


###Functions:

####getRandomAccent():
name: Name of the color

index: What index this accent is from

accent: The hexadecimal color code

light: Indicates if this color is light. It is recommended to match light colors backgrounds with black text.


    MaterialColor.getRandomAccent();
    //{ name: 'amber', index: 3, accent: '#ffab00', light: false }


####getRandomHue():
name: Name of the color

index: What index this accent is from

accent: The hexadecimal color code

light: indicates if this color is light. It is recommended to match light colors backgrounds with black text.


    MaterialColor.getRandomHue();
    //{ name: 'yellow', hue: '#fdd835', index: 6, light: false }


####getRandomColor():
name: Name of the color

hue.colors: An array of colors in descending shades.

hue.light: Indicates at what index the last light color is at.

accent.colors: An array of colors in descending shades.

accent.light: Indicates at what index the last light color is at.


    MaterialColor.getRandomColor();
    //{ name: 'yellow',
    //    hue:
    //     { light: 2,
    //       colors:
    //        [ '#fffde7',
    //          '#fff9c4',
    //          '#fff59d',
    //          '#fff176',
    //          '#ffee58',
    //          '#ffeb3b',
    //          '#fdd835',
    //          '#fbc02d',
    //          '#f9a825',
    //          '#f57f17' ] },
    //    accent:
    //     { light: 0,
    //       colors: [ '#ffff8d', '#ffff00', '#ffea00', '#ffd600' ] } }


