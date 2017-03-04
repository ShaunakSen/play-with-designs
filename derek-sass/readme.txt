SASS
___________

-> reuse code using vars
-> Compass: framework built on SASS
    CSS code:
        #div5:hover: {
            -webkit-transform: translateY(50%) scale(0.5);
            -moz-transform: translateY(50%) scale(0.5);
            -o-transform: translateY(50%) scale(0.5);
            -ms-transform: translateY(50%) scale(0.5);
            transform: translateY(50%) scale(0.5);
        }
    Compass:
        #div5:hover: {
            @include transform(translateY(50%) scale(0.5));
        }
-> Use nesting
    Css:
        #horNav a{
            color: white;
        }
        #horNav a:hover{
            color: red;
        }

    Sass:

        a{
            color:white
            &:hover{
                color: red;
            }
        }

-> Automatic Compression


Creating a compass project

compass create derek-sass

Inside config.rb:

# You can select your preferred output style here (can be overridden via the command line):
# output_style = :expanded or :nested or :compact or :compressed

compact: puts css in a single line
compressed: use for production.. removes comments, whitespaces etc

Also:

# Require any additional compass plugins here.

here we can require plugins



