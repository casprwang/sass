# SASS

```sass
// if
p {
  @if 1 + 1 == 2 { border: 1px solid;  }
  @if 5 < 3      { border: 2px dotted; }
  @if null       { border: 3px double; }
}


// if else
$type: monster;
p {
  @if $type == ocean {
    color: blue;
  } @else if $type == matador {
    color: red;
  } @else if $type == monster {
    color: green;
  } @else {
    color: black;
  }
}

//for
@for $i from 1 through 3 {
  .item-#{$i} { width: 2em * $i; }
}

//for each
@each $animal in puma, sea-slug, egret, salamander {
  .#{$animal}-icon {
    background-image: url('/images/#{$animal}.png');
  }
}

//while
$i: 6;
@while $i > 0 {
  .item-#{$i} { width: 2em * $i; }
  $i: $i - 2;
}


// & = this(parent)
@mixin does-parent-exist {
  @if &
    &:hover {
      color: red;
    }
  } @else {
    a {
      color: red;
    }
  }
}



```

nth($list, $n):
the nth() function in sass needs the position to starts at 1!!!
that's against with JS, little bit uncomfortable


```sass
// nav if it is in the header
nav {
	header & {
		background-color: darken($blue, 15%);
	}
```


ampersand &

clearfix should be a minxin and inclue whenever you have a float opeartion 
