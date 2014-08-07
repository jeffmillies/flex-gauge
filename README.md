FlexGauge
==========

Extremely customizable HTML5/jQuery Animated Gauge. Built to work with [RequireJS](http://requirejs.org/) or manually including the file.


Examples
========

[FlexGauge Examples](http://flexgauge.js.codethis.in)

[Drawing Arc](http://www.html5canvastutorials.com/tutorials/html5-canvas-arcs/) (Helpful for arcAngleStart and arcAngleEnd values)


Options
=======
        /**
         *  {String} Element that you would like to append to. ie '#idname', '.classname', 'div#idname', etc..
         */
        appendTo: 'body',
        /**
         *  {String} Id of Canvas already created or Id of canvas that will be created automatically
         */
        elementId: 'canvas',
        /**
         *  {String} Class of canvas created
         */
        elementClass: 'canvas',
        /**
         *  {Int} Canvas Width & Height
         */
        elementWidth: 200,
        elementHeight: 200,
        /**
         *  {Boolean|String} Generate Dial Value for the Gauge, true will use arcFillPercent or arcFillInt
         *  depending on provided values and specified dialUnits, string will use specified value
         */
        dialValue: false,
        /**
         *  {String} Class applied to div when dial is generated.
         */
        dialClass: 'fg-dial',
        /**
         *  {string: %|$| } Type of unit to use for the dial
         */
        dialUnit: '%',
        /**
         *  {string: before|after} Where the dial unit will be displayed
         */
        dialUnitPosition: 'after',
        /**
         *  {Boolean|String} Generate Label for the Gauge, true will use default "FlexGauge", string will use specified
         */
        dialLabel: false,
        /**
         *  {String} Class applied to div when label is generated.
         */
        dialLabelClass: 'fg-dial-label',
        /**
         *  {Int} Radius of the arc
         */
        arcSize: 85,
        /**
         *  {double} Starting and Ending location of the arc, End always needs to be larger
         *  arc(x, y, radius, startAngle, endAngle, anticlockwise)
         */
        arcAngleStart: 0.85,
        arcAngleEnd: 2.15,
        /**
         *  {double} Percentage the arc fills
         */
        arcFillPercent: .5,
        /**
         *  {Int} Starting and Ending values that are used to
         *  find a difference for amount of units
         *  ie: 60 (arcFillEnd) - 10 (arcFillStart) = 50
         */
        arcFillStart: null,
        arcFillEnd: null,
        /**
         *  {Int} Data used to find out what percentage of the
         *  arc to fill. arcFillInt can be populated by
         *  the difference of arcFillStart and arcFillEnd
         */
        arcFillInt: null,
        arcFillTotal: null,
        /**
         *  {Int} Color lightness: 0 - 255, 0 having no white added, 255 having all white and no color
         */
        arcBgColorLight: 80,
        /**
         *  {Int} Color saturation: 0 - 100, 0 having no color, 100 is full color
         */
        arcBgColorSat: 60,
        /**
         *  {Int} Size of the line marking the percentage
         */
        arcStrokeFg: 30,
        /**
         *  {Int} Size of the container holding the line
         */
        arcStrokeBg: 30,

        /**
         *  {string: hex} Color of the line marking the percentage
         */
        colorArcFg: '#5bc0de',
        /**
         *  {string: hex} Color of the container holding the line, default is using the Fg color and lightening it
         */
        colorArcBg: null,

        /**
         *  {String} Instead of providing a color or hex for the color, you can provide a class from the style
         *  sheet and specify what you would like to grab for the color in styleSrc
         */
        styleArcFg: null,
        styleArcBg: null,
        styleSrc: 'color',

        /**
         *  {Boolean} If set to false, then the graph will not be animated
         */
        animateEasing: true,
        /**
         *  {Int} Speed for the animation, 1 is fastest, higher the number, slower the animation
         */
        animateSpeed: 5,
        /**
         *  {Int} Math used in animation speed
         */
        animateNumerator: 12,
        animateDivisor: 15
