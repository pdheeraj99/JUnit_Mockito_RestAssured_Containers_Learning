JUnit 5 (JUnit Lambda) lo deenini "Modular Architecture" antaru.

Nuvvu cheppina points ni inka clarity kosam simple bullet points lo technical ga summarize chestunnanu:

* **JUnit Platform:** Idi oka **Base/Foundation** lantidi. Test frameworks run avvadaniki kavalsina infrastructure ni idi provide chestundi. Command line nunchi kani, IDE (IntelliJ) nunchi kani tests run avvalante deeni paine depend avtayi.
* **JUnit Jupiter:** Idi **Latest API**. Manam JUnit 5 lo kotha tests rayadaniki (annotations like `@Test`, `@BeforeEach`) deenine vaadutam. Indulo kotha engine kuda untundi.
* **JUnit Vintage:** Idi **Backward Compatibility** kosam. Nuvvu annattu, project lo patha JUnit 3 leda JUnit 4 tests unte, avi JUnit 5 platform meeda run avvadaniki idi help chestundi. 

### **JUnit 5 Architecture Diagram**

Nuvvu annattu idi ela work avutundo ee chinna ASCII diagram chudu mawa:

```text
       +----------------------------------------------------------+
       |                    JUnit Platform                        |
       |           (Launcher, IDE Support, Build Tools)           |
       +----------------------------------------------------------+
                /                     |                    \
               /                      |                     \
    +------------------+    +-------------------+    +-------------------+
    |  JUnit Jupiter   |    |   JUnit Vintage   |    |  Other Engines    |
    |  (New Junit 5)   |    | (Old Junit 3/4)   |    |  (Spock, etc.)    |
    +------------------+    +-------------------+    +-------------------+
```
