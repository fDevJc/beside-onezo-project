# CentOS7) MySQL μΈν

---

### πΒ λ²μ  νμΈ

```java
mysql --version
mysqld -V
```

### πΒ μλ² μ€ν

```java
systemctl enable mysqld && systemctl start mysqld && systemctl status mysqld
```

### πΒ μλ²μ€νμ ν¨μ€μλ νμΈ

```java
grep 'temporary password' /var/log/mysqld.log
ezA>ft1AWIur
```

### πΒ μλ² μ μ

```java
mysql -u root -p
```

### πΒ μλ² λ£¨νΈ ν¨μ€μλ λ³κ²½

```java
ALTER USER 'root'@'localhost' IDENTIFIED BY 'Onezo12#';
```

### πΒ λ°μ΄ν° λ² μ΄μ€ μμ±

```java
CREATE DATABASE db_live_god_life default CHARACTER SET UTF8;
```

### πΒ λ°μ΄ν° λ² μ΄μ€ μ­μ 

```java
DROP DATABASE <λ°μ΄ν°λ² μ΄μ€λͺ>;
```

### πΒ λ°μ΄ν° λ² μ΄μ€ λ¦¬μ€νΈ μ‘°ν

```java
SHOW DATABASES;
```

### πΒ μ¬μ©μ μΆκ°

```java
create user live_god_life@localhost identified by 'Onezo12#';
create user live_god_life@'%' identified by 'Onezo12#';
```

- λ€μ νΈμ€νΈλ IPμ μ νμ©μ΄λ μ°κ΄μμ.

### πΒ μ¬μ©μ λ¦¬μ€νΈ νμΈ

```java
use mysql;
select host,user,password from user;
```

### πΒ μ¬μ©μ κΆν λΆμ¬

```java
GRANT select,insert,update,delete ON db_live_god_life.* to live_god_life@'%';

GRANT select,insert,update,delete,create,alter,drop ON db_live_god_life.* to live_god_life@'%';
```

### πΒ μ¬μ©μ IP μ μκΆν

```java
λͺ¨λ  IP νμ©
GRANT ALL ON *.* TO live_god_life@'%';
```

### πΒ λ³κ²½ μ¬ν­ μ μ©

```java
FLUSH PRIVILEGES;
```

### πΒ PORT νμΈ

```java
SHOW GLOBAL VARIABLES LIKE 'PORT';
```

---

μΈν μλ¬

### π»Β Public Key Retrieval is not allowed

- DBeaver μ€μ λ³κ²½
- [https://deviscreen.tistory.com/85](https://deviscreen.tistory.com/85)

### π»Β ****You are not allowed to create a user with GRANT****

- [https://dzzienki.tistory.com/22](https://dzzienki.tistory.com/22)

### π»Β Host 'IP' is not allowed to connect to this MySQL serverβ

- [https://galid1.tistory.com/349](https://galid1.tistory.com/349)