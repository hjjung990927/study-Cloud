# **코리아 IT 아카데미 국비과정** 
## Cloud 😺
<a name="readme-top"></a> 


#### 설치 과정

  ubuntu
  
  sudo passwd
  
  1234
  
  su root / su ubuntu 
  
  	// 사용자 변경
	  
  sudo apt update && sudo apt upgrade -y
  
  date
  
  sudo apt install -y tzdata
  
  sudo dpkg-reconfigure tzdata
  
  export TZ=Asia/Seoul
  
  	// 한국 시간으로 설정
	  
  sudo apt install openjdk-17-jdk

  vim ~/.bashrc 
  
  	// 환경변수 설정
  	// 맨 밑으로 가서 (대문자 G)
	  
  export JAVA_HOME=$(dirname $(dirname $(readlink -f $(which java))))
  
  export PATH=$PATH:$JAVA_HOME/bin
  
  	// 복붙 후 esc 누르고 :wq
	
  source ~/.bashrc
  
  	// 변경한 설정 반영
	
  java -version
  
  javac -version
  
  	// 자바 버전 확인
	  
  sudo apt install mysql-server
  
  sudo systemctl start mysql
  
  sudo systemctl enable mysql
  
  sudo vim /etc/mysql/mysql.conf.d/mysqld.cnf
  
  sudo /etc/init.d/mysql restart
  
