AndroidResourceManager
======================

A set of classes to make accessing Android Resources easier and more consistent within your apps

Ideas;
# simple delegate to application's resources
# integrated Enum handling
# generated code from Resources
** Add namespaced attributes for resources to map 

```XML
<string name="foobar" lf:value="com.example.MyEnum.SOMEVALUE" lf:set="title">Some Value</string>
```

```java
ResourceManager manager = ResourceManager.get(getApplicationContext());
MyEnum value = MyEnum.SOMEVALUE;
String myEnumTitle = manager.getStringResource(value, "title");

```
