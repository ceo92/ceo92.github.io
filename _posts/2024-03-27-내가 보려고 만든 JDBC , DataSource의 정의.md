<html>
<head>
    <style>
        .text_color{
             background: rgb(255,0,0);
             background: linear-gradient(120deg, rgba(255,0,0,1) 0%,  rgba(245,255,0,1) 33.3%,
             rgba(34,106,42,1) 66.6%, rgba(4,37,240,1) 100%);
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
        
          
            <h3><b>JDBC 개념</b></h3>
      			<ul>
          		
 		        	<li><b style="color:#006600">커넥션 생성 , SQL 요청 , 결과 응답 추상화</b> : JDBC 표준 인터페이스</li>
 		         	<li><b style="color:#006600">커넥션 생성 , SQL 요청 , 결과 응답 구현체</b> : H2 드라이버 , Oracle 드라이버 , MySQL 드라이버</li>
                  <p><b>★ 각 db와 호환되는 각 드라이버가 있기에 자바에서 DB로 연결이 가능한 것!</b></p>
          		
      			</ul>
			<br><br>

           <h4><b>JDBC 결론</b></h4>
          		<ul>
                	<li><b style="color:#006600">드라이버</b> : 자바에서 각 드라이버와 연결하는 방법을 정의(커넥션 생성 => SQL 전달 => 결과 응답)</li>
                    <li><b style="color:#006600">JDBC</b> : 자바에서 각 드라이버와 연결하는 방법을 추상화시켜놓음</li>
		          <span>=> 구현체 유연하게 갈아끼우고 변경 가능하게</span>
      			</ul>  
            <br><br>
        
			
    </div>

    <hr>

    <div>
        
        <h3 class="text_color"><b>DataSource</b></h3>
        
            <h4><b>DataSource 개념</b></h4>
          <ul>
	          <li><b style="color:#006600">커넥션 생성 추상화</b> : DataSource</li>
    	      <li><b style="color:#006600">커넥션 생성 구현체</b> : 커넥션 풀 , DriverManager</li>
          </ul>
         <br><br>

          	<h4><b>DataSource 결론</b></h4>
      
	          <ul>
    	            <li>JDBC에서 DB와 연결하는 3가지 방법 중 첫 단추인 “커넥션 생성”하는 방법이 여러 가지가 있으니 그들을 DataSource라는 인터페이스로 추상화해놨음</li> 
        			<li>그에 다라 유연한 변경 가능</li>
	          </ul>
          
          <br><br>
         
       
    </div>
  
  		 <hr>	
  		
  
  <div>
    <h3 class="text_color"><b>결론</b></h3>
	    <ul>
    		<li>JDBC : 자바에서 DB와 <b style="color:red">1. 커넥션 생성</b> , <b style="color:blue">2. SQL 요청</b> , <b style="color:#006600">3. 결과 응답</b>하는 방법 추상화</li>
    		<li>DataSource : 자바에서 DB와 <b style="color:red">1. 커넥션 생성</b> 방법 추상화</li>
    	</ul>
  </div>
</div>

</body>
</html>
