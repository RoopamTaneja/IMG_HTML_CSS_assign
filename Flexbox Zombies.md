# Flexbox Zombies

## Chapter-1:
### Options used:
flex-direction:row (to point horizontally, ie EAST)
flex-direction: row-reverse (to point horizontally in reverse direction, ie WEST)
flex-direction: column (for pointing SOUTH)
flex-direction: column-reverse (for pointing NORTH)

## Chapter-2:
### Options used:
display:flex (to activate flexbox)
justify-content: flex-end (to align at horizontal end of flexbox)
(End implies farther from where main axis starts, which is different for different flex-directions)
(Like for flex-direction: column, aligns at vertical end of container and so on)

justify-content: center (for aligining to center)

justify-content: space-between (for equal space between elements but not at extreme ends)

justify-content: space-around (space between elements including extreme ends, but less at ends than between)

Tutorial part over, it's show time:

### 2.12 : 
flex-direction: row-reverse;
justify-content:flex-end;
(Aiming at end of flexbox while pointing west)

### 2.13:
flex-direction: column;
justify-content: center;
(Aiming at center of flexbox while pointing south)

### 2.14:
flex-direction: column-reverse;
(Aiming at beginning of flexbox while pointing north)

### 2.15:
flex-direction: column-reverse;
justify-content:space-between;
(Aiming at beginning of flexbox while pointing north with space only in between)

### 2.16:
flex-direction: column-reverse;
justify-content:center;
(Aiming at center of flexbox while pointing north)

### 2.17:
flex-direction:row-reverse;
justify-content:space-around;
(Aiming in west with space between elements including extreme ends, but less at ends than between)

Just realised, the levels are too many to add explanations for each of 'em, so just gonna add the codes now till the time they remain elementary.

### 2.18:
display: flex;
flex-direction:  column;
justify-content: flex-end;

### 2.19:
display: flex;
flex-direction:  row;
justify-content: center;

### 2.20:
display: flex;
flex-direction:  row-reverse;
justify-content: center;

## Chapter-3:
### 3.3:
align-items: flex-start;
(always perpendicular to justify-content, actual direction depends on flex-direction)
(like here it implies vertical alignment, top to bottom)

### 3.4:
flex-direction: column-reverse;
align-items: flex-start;
(always perpendicular to justify-content, actual direction depends on flex-direction)
(like here it implies horizontal alignment, left to right)

### 3.5:
align-items: flex-end;

### 3.6:
flex-direction: column;
align-items: flex-end;

### 3.7:
align-items:stretch;

### 3.8:
align-items: center;

### 3.10:
flex-direction: column-reverse;
  justify-content:flex-end;
  align-items:flex-end;

### 3.11:
flex-direction: row-reverse;
justify-content: space-between;
align-items: flex-start

### 3.12:
flex-direction: column;
justify-content: center;
align-items: center

### 3.13:
flex-direction: row-reverse;
justify-content: flex-end;
align-items: flex-end;

### 3.14:
flex-direction: column;
justify-content:space-around;
align-items: flex-start;

### 3.15:
flex-direction: column-reverse;
justify-content:flex-end;
align-items: flex-start;

### 3.16:
justify-content:center;
align-items: flex-start;

### 3.17:
justify-content:space-around;
align-items: flex-end;

### 3.18:
justify-content:space-between;
align-items: stretch;

### 3.19:
display:flex;
(coz everything else is default)

### 3.20:
flex-direction: row-reverse;
justify-content:flex-end;
align-items: center;

## Chapter-4:
### 4.3:
justify-content:flex-end;
align-items: center;

### 4.4:
```
crossbow {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

.target:nth-of-type(2) {
  align-self:flex-start;
}
```
(have all others be aligned center vertically except the second which is aligned at top vertically)

### 4.5:
```
.target:nth-of-type(1) {
  align-self:stretch;
}
```

### 4.6:
```
crossbow {
  display: flex;
  align-items: flex-start;
  flex-direction:row-reverse;
}

.target:nth-of-type(1) {
  align-self: center;
}
```
(due to row-reverse, the rightmost is actually no 1)

### 4.7:
```
.target.male {
  align-self:flex-end;
}
```
### 4.8:
```
.target:nth-of-type(2) {
  align-self:flex-end;
}
```
### 4.10:
```
crossbow {
  display:flex;
  justify-content:flex-end;
  align-items:flex-start;
}

.target:nth-of-type(2) {
  align-self:stretch;
  
}
```
### 4.11:
```
crossbow {
  display:flex;
  justify-content:space-between;
  align-items:flex-end;
}

.target:nth-of-type(2) {
  align-self:flex-start;
}
```
### 4.12:
```
crossbow {
    display:flex;
    flex-direction:column-reverse;
  align-items:flex-end;
}

.target.female {
  align-self:center;
}
```
### 4.13:
```
crossbow {
  display:flex;
  justify-content:space-around;
  
}

.target:nth-of-type(3) {
  align-self:flex-start;
  
}
```
### 4.14:
```
crossbow {
  display:flex;
  flex-direction:row-reverse;
  justify-content:center;
  align-items:center;
  
}

.target:nth-of-type(3) {
  align-self:flex-end;
  
}
```
### 4.15:
```
crossbow {
  display:flex;
  flex-direction:column-reverse;
  justify-content:space-between;
  align-items:center;
  
}

.target:nth-of-type(2) {
  align-self:flex-end;
  
}
```
### 4.16:
```
crossbow {
  display:flex;
  flex-direction:row-reverse;
  justify-content:flex-end;
  align-items:flex-end;
  
}

.target:nth-of-type(3) {
  align-self:flex-start;
  
}
```
### 4.17:
```
crossbow {
   display:flex;
  justify-content:center;
  align-items:center;
}
.target.female {
  align-self:flex-start;

}
```

*Backticks seem fun but are tiring, so no more backticks*

## Chapter-5:
### 5.5:
display:flex;
  justify-content:center;
  align-items:center;

### 5.6:
  crossbow {
  display: flex;
  justify-content: center;
  align-items: center;
}

.target.goo {
  flex-grow:1;
}

### 5.7:
flex-grow:1;
(flex-grow makes stuff grow vertically if we're aiming north or south)

### 5.8:
.target:nth-of-type(1) {
    flex-grow:1;
}

.target:nth-of-type(2) {
  flex-grow:2;
  
}
(bcoz the second one grew at **twice the rate** as first one)

### 5.9:
.target:nth-of-type(1) {
  flex-grow: 3;
}

.target:nth-of-type(2) {
  flex-grow: 1;
}

### 5.10:
crossbow {
  display: flex;
  justify-content: center;
  align-items: center;
}

.target{
  flex-grow:1;
}

.target:nth-of-type(2) {
  flex-grow:0;
}
(flex-grow always acts on flex items and can be overriden if needed)

### 5.12:
crossbow {
  display: flex;
}

.target.goo {
  flex-grow:1;
  align-self:flex-end;
  
}

.target.female {
  align-self:flex-start;
}

### 5.13:
crossbow {
  display: flex;
  flex-direction:column;

}

.target:nth-of-type(1) {
}

.target:nth-of-type(2) {
  align-self:flex-end;
  flex-grow:1
  
}

### 5.14:
crossbow {
  display:flex;
  flex-direction:row-reverse;
  align-items:center;
}

.target.goo {
  flex-grow:1;
}

.target:nth-of-type(1) {
  flex-grow:2;
  align-self:flex-end;
  
}

### 5.15:
crossbow {
  display:flex;
  flex-direction:column-reverse;
  align-items:flex-start;
}

.target:nth-of-type(3) {
  flex-grow:1;
}

### 5.16:
crossbow {
  display:flex;
  align-items:flex-start;
}

.target.goo {
  flex-grow:1;
  align-self:stretch;
}

### 5.17:
crossbow {
  display:flex;
  flex-direction:row-reverse;
  align-items:flex-start;
}

.target.goo {
  flex-grow:1;
}

.target:nth-of-type(1) {
  flex-grow:0;
}

.target:nth-of-type(4) {
  flex-grow:3;
}

### 5.18:
crossbow {
  display:flex;
  flex-direction:column-reverse;
  align-items:center;
}

.target.goo {
  flex-grow:1;
}

.target:nth-of-type(2) {
  align-self:stretch;
}

.target:nth-of-type(3) {
  flex-grow:0;
}

### 5.19:
crossbow {
  display:flex;
  align-items:flex-end;
}

.target.goo {
 flex-grow:1;
 align-self:flex-start;
}

.target:nth-of-type(3) {
 align-self:stretch 
}

### 5.20:
crossbow {
  display:flex;
  flex-direction:row-reverse;
  align-items:flex-end;
}

.target.goo {
  flex-grow:1;
}

.target:nth-of-type(4) {
  flex-grow:3;
}

### 5.21:
crossbow {
  display:flex;
  flex-direction:column;
  align-items:flex-end;
}

.target:nth-of-type(2) {
  flex-grow:1;
  align-self:stretch;
}

## Chapter-6:
### 6.3:
.target.goo {
  flex-shrink:1;
}

### 6.4:
.target.goo {
  flex-shrink:2;
}

6.5:
.target:nth-of-type(2), .target:nth-of-type(3) {
  flex-shrink:2;
}

6.6:
.target:nth-of-type(3) {
  flex-shrink:3
}

6.7:
.target:nth-of-type(3) {
  flex-shrink:0;
}

6.8:
.target.goo {
  flex-grow:1;
}

6.10:
crossbow {
  display:flex;
  align-items:flex-start;
}

.target.goo {
  flex-grow:1;
}

.target.male {
  align-self:center;
}

6.11:
