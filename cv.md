# Yauhen Kalanitski
### Contacts
- **phone**: +375(29)254-07-79;
- **email**: kolonicki.e@gmail.com;
- **telegram**: @DrD1esel;

### Summary
My main goal is to get a job as a front-end developer. I want this because programming much more attractive to me than my current field of activity. I spend all my free time to increase programming and English skills to reach my main goal.

### Skills
Basic knowledge of HTML, CSS, JavaScript, Git & GitHub, Java, SQL.
### Latest code example
```javascript
function sudoku(puzzle) { 
  var sudoku=puzzle.map(x=>{return x.join("")}).join(",")  
  return next(sudoku).split(",").map(x=>{ return x.split("").map(z=>{return +z})})
}

function getPossibleDigits(row,column,str){
    var array=str.split(",")
    var hor=array[row]
    var ver=array.map(x=>{return x.charAt(column)})
    var sqrRow=Math.floor(row/3)*3
    var sqrColumn=Math.floor(column/3)*3    
    var sqr=[0,1,2].map(x=>{return array[sqrRow+x].substr(sqrColumn,3)}).join("")    
    return "123456789".replace(new RegExp("["+hor+ver+sqr+"]","g") ,"").split("")
}

function next(str){    
    var index = str.replace(/,/g,"").indexOf("0")
    if (index==-1) return str    
    var digits = getPossibleDigits(Math.floor(index/9),index%9,str)
    if (!digits[0]) return false 
    for (var i=0;i<digits.length; i++){      
      var temp = str.replace("0",digits[i])     
      var ch = next(temp)
      if(ch) return ch
    }    
}
```
### Experience
- course and graduation projects at the university;
- two times participated in Itransition Opener competitions (both of them finished in Top-100)

### Education
- Belarusian State Economic University(2013);
- Belarusian State University of Informatics and Radioelectronics(2019)

### English
Pre-intermediate