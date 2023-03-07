### choose
junit
mockito
powermock
TestNG
EasyMock

#### Mockito
##### mock有返回值方法

``` java
@MockBean(org.springframework.boot.test.mock.mockito)
private XX xx;

Mockito.when(xx.aa()).thenReturn(..);
```

##### mock无返回值方法
``` java
org.mockito.Mockito.doNothing().when(xx).xxmethod();
```

##### 设置成员变量的属性
``` java
org.springframework.test.util.ReflectionTestUtils.setField(xxInstance, "xxfield", "xxval");
```
