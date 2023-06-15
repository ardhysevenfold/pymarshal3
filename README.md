# Stealthify V2

Stealthify V2 is a lightweight code obfuscator for Python, designed to provide basic protection against casual reverse engineering of your source code.
It applies simple obfuscation techniques to make your code less readable and deter unauthorized access.

# Features:
- Basic Name Obfuscation: Stealthify V2 renames variables, functions and class names with randomly generated names to make the code less intuitive.
- The obfuscated code is enhanced with randomly generated lines of junk code, which are interspersed throughout the code to make it more difficult to analyze and understand.
- Limited AST Transformations: The obfuscator performs basic Abstract Syntax Tree (AST) transformations to modify the code structure and confuse potential attackers.
- Another Encoding layer: Adds another layer of Base64, base85, marshal and lzma Encoding and compression over the obfuscated code to make it slightly harder to understand. It uses some code from Codeuk on Github. Go check him out!
- Add startup code that lets you run that script on startup.
- Multiple Obfuscation Layers: You can choose to apply multiple layers of obfuscation to the code to make it slightly harder to understand.
- Basic Anti-VM code to bypass Virtual Machine Environments.

# Example
Before:
```python
class Circle:
    def __init__(self, radius):
        self.radius = radius

    def calculate_area(self):
        return 3.14 * self.radius ** 2
area = Circle.calculate_area()
print("Area:", area)
```
After:
```python
# Obfuscated With Stealthify V2 By Sirmilann
class IIlIlllIlIllIlIllIlIIIll:

    def __init__(lllIlIlIIIlIIlIIlIl, lIIlIIlIlIIIllIl):
        lllIlIlIIIlIIlIIlIl.radius = lIIlIIlIlIIIllIl

    def calculate_area(lllIlIlIIIlIIlIIlIl):
        return 3.14 * lllIlIlIIIlIIlIIlIl.radius ** 2
IIlIlIIllIllIllIII = IIlIlllIlIllIlIllIlIIIll.calculate_area()
print('Area:', IIlIlIIllIllIllIII)
```
After Including Junk Code:
```python
# Obfuscated With Stealthify V2 By Sirmilann
class IlIlIlIllIlllIIlIIllIlI:
#__STEALTHIFY_V2____STEALTHIFY_V2__
    def __init__(IIlIIIIIlllllll, IIllllllIIIlIlIII):
#__STEALTHIFY_V2____STEALTHIFY_V2__
        IIlIIIIIlllllll.radius = IIllllllIIIlIlIII
#__STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2__
    def calculate_area(IIlIIIIIlllllll):
#__STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2__
        return 3.14 * IIlIIIIIlllllll.radius ** 2
#__STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2__
IllIlIlllIIlIllIII = IlIlIlIllIlllIIlIIllIlI.calculate_area()
#__STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2____STEALTHIFY_V2__
print('Area:', IllIlIlllIIlIllIII)
#__STEALTHIFY_V2____STEALTHIFY_V2__
```
After Encoding And Compression:
```python
# Obfuscated With Stealthify V2 By Sirmilann
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ = ""
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "YyR8SFolTD"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "5DRjVKbDZp"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "VW9wRXhETU"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "JBQkEmVn5r"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "aEF1Pm0xIT"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "BpbDxOckhK"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "bGVWTzN1Wn"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "0zKD5scjNy"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "Y1RNQmE8X3"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "VhUkVqPF5W"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "TllZdnsyQm"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "c4P3o/Y3cy"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "RntXRXdfO1"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "MrVDFKMlFC"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "a2dpLSEqLU"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "BKam5kfWcx"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "aFc8UEhyYU"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "Z0UnFBbExv"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "PG4xPjUxQy"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "lISkRaKXR9"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "JkxJOXtnQD"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "dZTk03Plph"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "NHxWZm42bX"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "IhSFhaSTlo"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "PkRtanVSNj"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "dufV4lczh0"
__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__ += "X0RnT3k="
exec(__import__('marshal').loads(__import__('zlib').decompress(__import__('base64').b85decode(__import__('base64').b64decode(__STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2____STEALTHIFY__V2__.encode()).decode()))))
```


# Usage:
1. Run the Stealthify V2 script.
2. Enter the path to the Python file you want to obfuscate.
4. Specify the number of obfuscation layers to apply.
5. Choose if you want to add junk code.
6. Choose if you want to use an extra encoding and compression layer.
7. Choose if you want to add anti vm code.
8. Choose if you want to use a startup method.
9. The obfuscated code will be saved to a new file with "_obf" appended to the original filename.

Please note that while obfuscation can provide a basic level of code protection, it does not guarantee absolute security.
attackers may still attempt to reverse engineer the code given time and expertise.

# Requirements
Python 3.x

# Licence
Stealthify V2 is released under the MIT License.
