1.

const square = function(x, y,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 4) {
        forward(length)
        right(90)
        i = i + 1
     }
}
2.
const rect = function(x, y,w,h) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 2) {
        forward(w)
        right(90)
        forward(h)
        right(90)
        i = i + 1
     }
}

3，

const square = function(x, y,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 4) {
        forward(length)
        right(90)
        i = i + 1
     }
}
const square5=function(){
    var a=0
    var b=0
    var j=0
    while(j<5){
        jump(a,b)
        square(a,b,30)
        a=a+30
        j=j+1
    }
}
4，
const square = function(x, y,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 4) {
        forward(length)
        right(90)
        i = i + 1
     }
}
const square5_10=function(){
    var a=0
    var b=0
    var j=0
    while(j<5){
        jump(a,b)
        square(a,b,30)
        a=a+40
        j=j+1
    }
}
5。
const square = function(x, y,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 4) {
        forward(length)
        right(90)
        i = i + 1
     }
}
const square_line=function(x,y,n,space,len){
    var a=x
    var b=y
    var j=0
    while(j<n){
        jump(a,b)
        square(a,b,len)
        a=a+len+space
        j=j+1
    }
} 
6.

const square = function(x, y,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 4) {
        forward(length)
        right(90)
        i = i + 1
     }
}
const square_line=function(x,y,n,space,len){
    var a=x
    var b=y
    var j=0
    while(j<n){
        jump(a,b)
        square(a,b,len)
        a=a+len+space
        j=j+1
    }
}
const square_square=function(x,y,space,len,n,m){
    var j=0
    var a=0
    var b=y
    while(j<m){
        square_line(x,y,n,space,len)
        b=b+len+space
        y=b
        j=j+1
    }
}
7.
const rect = function(x,y,w,h) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 2) {
        forward(w)
        right(90)
        forward(h)
        right(90)
        i = i + 1
     }
}
const rect_line=function(x,y,w,h,n,space){
    var a=x
    var b=y
    var j=0
    while(j<n){
        jump(a,b)
        rect(a,b,w,h)
        a=a+w+space
        j=j+1
    }
} 
8.

const rect = function(x,y,w,h) {
    jump(x, y)
    setHeading(0)
    var i = 0
    while (i < 2) {
        forward(w)
        right(90)
        forward(h)
        right(90)
        i = i + 1
     }
}
const rect_line=function(x,y,w,h,n,space){
    var a=x
    var b=y
    var j=0
    while(j<n){
        jump(a,b)
        rect(a,b,w,h)
        a=a+w+space
        j=j+1
    }
} 
const rect_square=function(x,y,space,w,h,n,m){
    var j=0
    var a=0
    var b=0
    while(j<m){
        b=y
        rect_line(x,y,w,h,n,space)
        b=b+h+space
        y=b
        j=j+1
    }
}
9.

const polygon= function(x, y,n,length) {
    jump(x, y)
    setHeading(0)
    var i = 0
    var angle=180-(n-2)*180/n
    while (i < n) {
        forward(length)
        right(angle)
        i = i + 1
     }
}
polygon(-100,-100,7,90)
