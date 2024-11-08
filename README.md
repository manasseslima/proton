# proton
A modern programing language


An example

```
import math: power, round
import net: http


Forms = enm() {
	POINT
	RECTANGLE
	TRIANGLE
	CIRCLE
}

Geomery = cls() {}

Point = cls() {
	x := 0
	y := 0
	
	distance = fnc() float {}
}

Rectangle = cls(Geometry) {
	height: flt
	width: flt
	
	__new__ = fnc(){}
	
	__init__ = fnc(height: flt, width: flt){
		slf.height = height
		slf.width = width
	}
	
	perimeter: fnc = () flt {
		rtn (slf.height + slf.width) * 2
	}
	
	area = fnc() flt {
		rtn slf.height + slf.width
	}
}

sum = fnc(n1: int, n2: int) int {
	rtn n1 + n2
}

div = fnc(num, den: flt) flt {
	if den == 0 {
		rtn inf
	}
	rtn num / den
}

Generys = enm() {
	STRATEGY
	COLABORATIVE
}

Game = stc() {
	name: str
	year: int
	genery: Generys
}

todo = fnc() {
	adct := {'name': 'Amanda Clark', 'salary': 1200.0}
	print(adct.name, adct.salary)
	amap := <'name': 'Igor Backary', 'salary': 1200.0>
	print(amap['name'])
}


main = fnc() int {
	n1 := 2
	n2 := 5
	res := sum(2, 3)
	print('A soma de {n1} + {n2} = {res}')
	rtn 0
}
```