HSUViewFrameHelpers
===================

Convenient methods to set UIView's frame

Check everything in the header file.

    #import <UIKit/UIKit.h>

    #define ccr(x, y, w, h) CGRectMake(floorf(x), floorf(y), floorf(w), floorf(h))
    #define ccp(x, y) CGPointMake(floorf(x), floorf(y))
    #define ccs(w, h) CGSizeMake(floorf(w), floorf(h))
    #define edi(top, left, bottom, right) UIEdgeInsetsMake(floorf(top), floorf(left), floorf(bottom), floorf(right))

    @interface UIView (Additions)

    @property (nonatomic, readwrite) CGFloat left, right, top, bottom, width, height;
    @property (nonatomic, readwrite) CGPoint topCenter, bottomCenter, leftCenter, rightCenter;
    @property (nonatomic, readwrite) CGPoint leftTop, leftBottom, rightTop, rightBottom;
    @property (nonatomic, readonly) CGPoint boundsCenter;
    @property (nonatomic, readwrite) CGSize size;

    - (NSString *)frameStr;

    @end

