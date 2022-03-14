# jsp_14 : 변수의 범위

![image](https://user-images.githubusercontent.com/37132897/158129208-418cd373-5a32-4fcc-802c-1e6254e34b71.png)


      var i = 10;
      
      if (i > 5) {
      
        var j = 100;
        
      } else {
      
        var j = 1000;
        
      }
      
      document.write(j);

      // var은 Funtion Scope 를 가지고, let,const 는 같은 블록상에 있어야만 사용가능하다.
      
      // var은 function 안에서는 사용이 안된다. 밖에 있는 var 변수를 가져와서, function 안에서 계산은 가능하다.
      
