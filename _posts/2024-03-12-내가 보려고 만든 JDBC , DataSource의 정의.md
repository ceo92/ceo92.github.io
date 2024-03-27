<html>
<head>
    <style>
        .text_color{
             background: rgb(255,0,0);
             background: linear-gradient(120deg, rgba(255,0,0,1) 0%, rgba(255,141,0,1) 17%, 			rgba(245,255,0,1) 34%,
             rgba(34,106,42,1) 51%, rgba(4,37,240,1) 68%, rgba(13,27,147,1) 85%, rgba(94,0,255,1) 100%);
        background-clip: text;
              -webkit-background-clip: text;
                color: transparent;
                }
    </style>
</head>

<body>
<div>
 
    <div>
        <h2 class="text_color"><b>JDBC</b></h2>
        <ul>
          
            <h4><b>JDBC 개념</b></h4>
          		
 		        	<li><b style="color:#006600">커넥션 생성 , SQL 요청 , 결과 응답 추상화</b> : JDBC 표준 인터페이스</li>
 		         	<li><b style="color:#006600">커넥션 생성 , SQL 요청 , 결과 응답 구현체</b> : H2 드라이버 , Oracle 드라이버 , MySQL 드라이버</li>
        		  	<li><b>★ 각 db와 호환되는 각 드라이버가 있기에 자바에서 DB로 연결이 가능한 것!</b></li>
          		
          
			<br><br>

           <h4><b>JDBC 결론</b></h4>
          		<div>
                	<span><b style="color:#006600">드라이버</b> : 자바에서 각 드라이버와 연결하는 방법을 정의(커넥션 생성 => SQL 전달 => 결과 응답)</span>
                    <span><b style="color:#006600">JDBC</b> : 자바에서 각 드라이버와 연결하는 방법을 추상화시켜놓음</span>
		          <span>=> 구현체 유연하게 갈아끼우고 변경 가능하게</span>
          
            <br><br>
        </ul>
			
    </div>

    <hr>

    <div>
        
        <h2 class="text_color"><b>DataSource</b></h2>
        <ul>
            <h4><b>DataSource 개념</b></h4>
          <div>
	          <span><b style="color:#006600">커넥션 생성 추상화</b> : DataSource</span>
    	      <span><b style="color:#006600">커넥션 생성 구현체</b> : 커넥션 풀 , DriverManager</span>
          </div>
         <br><br>

          	<h4><b>DataSource 결론</b></h4>
	          <div>
    	            <span>- JDBC에서 DB와 연결하는 3가지 방법 중 첫 단추인 “커넥션 생성”하는 방법이 여러 가지가 있으니 그들을 DataSource라는 인터페이스로 추상화해놨음</span> 
        			<span>- 그에 다라 유연한 변경 가능</span>
	          </div>
          
          <br><br>
         
        </ul>
    </div>
  
  		 <hr>	
  		
  
  <div>
    <h2 class="text_color"><b>결론</b></h2>
	    <div>
    		<span>JDBC : 자바에서 DB와 <b style="color:red">1. 커넥션 생성</b> , <b style="color:blue">2. SQL 요청</b> , <b style="color:#006600">3. 결과 응답</b>하는 방법 추상화</span>
    		<span>DataSource : 자바에서 DB와 <b style="color:red">1. 커넥션 생성</b> 방법 추상화</span>
    	</div>
  </div>
</div>

</body>
</html>
