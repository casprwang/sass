# SASS

* Pre-processed
* Extensible
* Written in Ruby
* Nesting
* Operations
* Minxins (like adding JS)
* Syntax
  * .sass (no punctuations)
  * .scss (with punctuations)



~~~Sass

$main_color : rgb(110, 17, 233);

/*Core Partial */
@import "base";

/*Import Moudule*/
@import "modules/nav"

/*extend*/
.btn-reverse {
  @extend .btn;
  background: rgb(99, 11, 156);
}

/*Operations*/
@if {

} @else {

}
~~~
