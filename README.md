# cyber-vector-notation

This is a **"NOTATION"** for those who use computers.  

Commentary by author:  

📖 [電脳記数法 (Cyber Number Notation)](https://crieit.net/posts/Cyber-Number-Notation)  

# Two prior knowledge

📖 [dictionary-ordinal-number-notation](https://github.com/muzudho/dictionary-ordinal-number-notation)  
📖 [beads-vector-notation](https://github.com/muzudho/beads-vector-notation)  

# Install

```shell
# pip install dicordnum
# pip install beadsvec
pip install cybervec
```

# Methods

## trail_zero() operation

With trailing zero  

👇 Append `,0`  

```plaintext
cn = CyberVec.trail_zero((1, 2))
print(f"{cn.elements}")                # (1, 2, 0)

cn = CyberVec.trail_zero(3)
print(f"{cn.elements}")                # (3, 0)
```

👇 Same  

```plaintext
cn = CyberVec((1, 2, 0))
print(f"{cn.elements}")                # (1, 2, 0)

cn = CyberVec((3, 0))
print(f"{cn.elements}")                # (3, 0)
```

# Let's give an example

## Cons

* It's eccentric

👇 Pre-zero cannot be used  

```plaintext
# Normal
0001

# Cyber
O1o0
```

👇 Hexadecimal cannot be used  

```plaintext
# Normal
0xFF

# Cyber
O255o0            # Use decimal
```

## Pros

* It is considered to be used for variable names, class names, method names, file names, folder names, URLs, etc.
* Use as dictionary ordinal number

👇 For Version number  

```plaintext
# Normal
Version1.0.1

# Cyber
VersionO1o0o1o0   # Default
VersionO1o0o1o0   # PascalCase
versionO1o0o1o0   # lowerCamelCase
version_o1o0o1o0  # snake_case
version-o1o0o1o0  # kebab-case
VERSION_O1O0O1O0  # UPPER_SNAKE_CASE
```

👇 For IPv4  

```plaintext
# Normal
128.0.0.1

# Cyber
OAA128o0o0o1o0  # Default
Oaa128o0o0o1o0  # PascalCase
oaa128o0o0o1o0  # lowerCamelCase
oaa128o0o0o1o0  # snake_case
oaa128o0o0o1o0  # kebab-case
OAA128O0O0O1O0  # UPPER_SNAKE_CASE
```

👇 Negative number included  

```plaintext
# Normal
20, 18, -1, -14, 5

# Cyber
OA20oA18o_9o__86o5  # Default
Oa20oa18o_9o__86o5  # PascalCase (Bad)
oa20oa18o_9o__86o5  # lowerCamelCase (Bad)
oa20oa18o_9o__86o5  # snake_case
oa20oa18o_9o__86o5  # kebab-case (Bad)
OA20OA18O_9O__86O5  # UPPER_SNAKE_CASE
```

👇 Folder

```plaintext
# Normal
📂 00
└── 📂 01
  └── 📂 99

# Normal Flat by "/"
00/01/99

# Cyber
📂 O0o0          # Not O00o0
└── 📂 O1o0
  └── 📂 OA99o0

// # **TODO** Cyber Flat by "o00o"
// O0o0o00oO1o0x1xOA99o0
```

👇 Chapter

```plaintext
# Normal
1. Food
1.1. Fruits
1.1.1. Apple
1.1.2. Banana
1.1.11. Kiwi

# Cyber
O1o0. Food
O1o1o0. Fruits
O1o1o1o0. Apple
O1o1o2o0. Banana
O1o1oA11o0. Kiwi
```

Now you have mastered cyber vector notation  
