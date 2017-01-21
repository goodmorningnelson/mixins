mixins


// ANIMATION MIXINS -> animation class based animation (ng-class) --- start


  @mixin animTowards($added-css-class) {
    //define final state
    &.#{$added-css-class}, &.#{$added-css-class}-add {
      @content;
    }
  }

  @mixin animReturn($added-css-class) {
    //redifine original state
    &.#{$added-css-class}-remove {
      @content;
    }
  }

// ANIMATION MIXINS -> animation class based animation (ng-class) --- end
