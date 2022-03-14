# jsp_14 : 변수의 범위

![image](https://user-images.githubusercontent.com/37132897/158129208-418cd373-5a32-4fcc-802c-1e6254e34b71.png)
- i는 10으로, 5보다 크기 때문에, j값이 100으로 출력된다. 여기서 var 대신, let 이나 const 로 사용 불가하다. 만약 사용하려면,

      var i = 10;
      
      // let j = 150; 처럼 출력문과 같은 블록에서, 선언해서 불러와야 한다. if문 안과, 바깥의 j 출력문은 다른 블록으로 보기 때문.
      
      if (i > 5) {
      
        var j = 100;
        
      } else {
      
        var j = 1000;
        
      }
      
      document.write(j);

      // var은 Funtion Scope 를 가지고, let,const 는 같은 블록상에 있어야만 사용가능하다.
      
      // var은 function 안에서는 사용이 안된다. 밖에 있는 var 변수를 가져와서, function 안에서 계산은 가능하다.
      
