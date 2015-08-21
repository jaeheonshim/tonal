# list 




## areIntervals() 

Given a list, check it its a interval list






### Returns


- `Void`




## areIntervals() 

Given a list, check it its a note list






### Returns


- `Void`




## chromaticList(length) 

Returns a interval list with a chromatic scale

The harmonic chromatic scale is the same whether rising or falling and
includes all the notes in the major, harmonic minor or melodic minor
scales plus flattened second and sharpened fourth degrees


### Parameters

- **length** `Integer`   - the number of items in the list




### Returns


- `Array`   a list (of intervals or notes, depending of params)




## distance() 








### Returns


- `Void`




## isBinaryList(number) 

Determine if a given number is a valid binary list number

A valid binary list is any binary number that starts with 1 (P1 interval)
The binary number can be expressed in decimal


### Parameters

- **number** `String`   - the number to test




### Examples

```javascript
isBinary('100') // => true
isBinaryList(2773) // => true
isBinaryList('010') // => false
```


### Returns


- `boolean`   true if its a valid scale binary number




## list(list) 

Get a list of notes or isInterval

This is the principal function to create lists. Basically does the same as
`list/parse` but if an array is given, it returns it without modification
or validation (so, only pass an array when you are sure that is a valid list)


### Parameters

- **list** `String` `Array`   - the list to be parsed or passed




### Examples

```javascript
list('c d# e5') // => ['C4', 'D#4', 'E5']
list('P1 m2') // => ['P1', 'm2']
list('bb2') // => ['Bb2']
list('101') // => ['P1', 'M2']
// to validate an array
list(['C#3', 'P2'].join(' ')) // => null
```


### Returns


- `Array`   an array list of notes or intervals (or anything it you pass an array to the function)




## transpose() 








### Returns


- `Void`




## parse(list) 

Parse a string to a note or interval list

The string can be notes or intervals separated by white spaces or a binary
or decimal representation of a interval list


### Parameters

- **list** `String` `Integer`   - the string to be parsed




### Returns


- `Array`   an array of notes or intervals, null if not valid list




## module.exports() 

Get the retrograde of a set

Alias of set/reverse




### Returns


- `Void`




## reverse(list) 

Get the reverse (retrograde) of a list




### Parameters

- **list** `String` `Array` `Integer`   - the list to be reversed




### Examples

```javascript
reverse('A B C') // => ['C', 'B', 'A']
```


### Returns


- `Array`   The reversed list




## rotate() 

Rotate a list






### Returns


- `Void`




*Documentation generated with [doxdox](https://github.com/neogeek/doxdox).*