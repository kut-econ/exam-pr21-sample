# プログラミング2021 期末試験

## Q1

1MiBは何KiBですか？答えなさい。

## Q2

次のうち、正しい記述には○を、誤った記述には×をつけなさい。(部分点あり)

1. アセンブルは可逆変換である。
2. CPythonはPythonにC言語の特徴を取り入れたコンパイル型言語である。
3. スクリプトからバイトコードを生成することをバイトコンパイルという。
4. RやJavaScriptはインタープリタ型言語である。
5. マシン語からアセンブリ言語のコードを生成することをアセンブルと呼ぶ。

## Q3

10進数の1000を16進ダンプした際に得られる表示はどれか？正しい選択肢の番号を答えなさい。ただしリトルエンディアン格納方式の2バイト整数とする。

1. 8e30
2. 308e
3. e803
4. 03e8

## Q4

負の数-2000を2の補数で表現したものは次のうちどれか?正しい選択肢を一つ選び、その番号を答えなさい。ただし2バイト整数でビッグエンディアン表記を用いることとする。

1. 11111000 00110000
2. 00000111 11010000
3. 10000111 11010000
4. 11111000 00101111

## Q5

27.625を単精度浮動小数点としてビット列表記したものは次のうちどれか。正しい選択肢を一つ選び、その番号を答えなさい。

1. 0-10000011-11011101 00000000 0000000
2. 0-00000100-10111010 00000000 0000000
3. 0-10000011-10111010 00000000 0000000
4. 0-00000100-11011101 00000000 0000000

<div style="page-break-before:always"></div>

## Q6

Git/Githubに関する問題です。Github上のリモートリポジトリrepoは唯一のブランチmasterを持っているとします。これを自身のパソコン上にクローンしてローカルリポジトリrepoを作成したとします。ローカルのrepo内で次の一連のコマンドを実行したあと、リモートとローカルの状態として正しいものを一つ選びなさい。

```bash
git branch new
git checkout new
git push -u origin new
git checkout master
git branch -d new
git push origin :new
```

1. リモート、ローカルともにmasterブランチのみが存在
2. リモートはmasterのみ、ローカルはnewのみが存在
3. リモートはmasterのみ、ローカルはmasterとnewが存在
4. リモートはmasterとnew、ローカルはmasterのみが存在
5. リモート、ローカルともにmasterとnewが存在

## Q7

Git/Githubに関する問題です。ローカルリポジトリrepo内に存在するファイルcode.pyに編集を加えたあと、ステージングしたとします(まだコミットはしていません)。このステージングをキャンセルし、ステージングする前の状態に戻すためのコマンドとして正しいものを一つ選びなさい。

1. git reset --hard HEAD
2. git reset --soft HEAD^
3. git reset --mixed HEAD^
4. git reset

## Q8

Git/Githubに関する問題です。ローカルリポジトリrepo内で4つのコミットcommit0, commit1, commit2, commit3を行ったとする。次のようにrevertコマンドを3回連続で実行したあと、作業エリアの状態として正しいものを一つ選びなさい。

```bash
git revert HEAD
git revert HEAD
git revert HEAD
```

1. commit0と同じ内容
2. commit1と同じ内容
3. commit2と同じ内容
4. commit3と同じ内容

<div style="page-break-before:always"></div>

## Q9

Git/Githubに関する問題です。ローカルリポジトリrepo内で4つのコミットcommit0, commit1, commit2, commit3を行った直後、次のコマンドを続けて実行したとします。

```bash
git reset --soft HEAD^
git reset --hard HEAD
```

このあと、作業エリアの状態として正しいものを一つ選びなさい。

1. commit0と同じ内容
2. commit1と同じ内容
3. commit2と同じ内容
4. commit3と同じ内容

## Q10

次のRコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```R
x <- c(1,2,3)
y <- x
x[2] <- 0
y[1] <- 6
print(x)
```

1. `[1] 1 2 0`
2. `[1] 6 0 3`
3. `[1] 1 6 0`
4. `[1] 1 0 3`

## Q11

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [1,2,3]
y = x
y.append(4)
print(x,x is y)
```

1. `[1,2,3,4] True`
2. `[1,2,3,4] False`
3. `[1,2,3] True`
4. `[1,2,3] False`

<div style="page-break-before:always"></div>

## Q12

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [1,2,3]
y = x[:]
z = y
y[:] = [4,5,6]
print(x,y,z)
```

1. `[4,5,6] [4,5,6] [4,5,6]`
2. `[1,2,3] [4,5,6] [4,5,6]`
3. `[4,5,6] [4,5,6] [1,2,3]`
4. `[1,2,3] [4,5,6] [1,2,3]`

## Q13

次のPythonコードを実行したあと、続けて実行したときにエラーが出ないコードには○を、エラーが出るコードには☓をつけなさい。(部分点あり)

```python
x = "Julia"
```

1. `x[-1] = "A"`
2. `y = x[4]`
3. `y = 3 * x`
4. `y = x[-1:-3:-1]`
5. `x = "Python"`
6. `x[:] == 'Python'`
7. `y = x + 5`
8. `x = x + x`
9. `x[0:1] = "Py"`

<div style="page-break-before:always"></div>

## Q14

次のRコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```R
library(pryr)
x <- c(1,2,3)
add <- address(x)
y <- x
z <- x
x[1] <- 4
print(c(address(x) == add, address(y) == add, address(z) == add))
```

1. `[1] TRUE FALSE FALSE`
2. `[1] TRUE TRUE TRUE`
3. `[1] FALSE FALSE FALSE`
4. `[1] FALSE TRUE TRUE`

## Q15

次のPythonコードを実行した際に、変数xに格納されている値を整数値で答えなさい。ただしリストのオーバーヘッド(=`sys.getsizeof([])`の戻り値)を56バイトとし、処理系は64ビットとする。

```python
import sys
x = sys.getsizeof([0,['Py','thon'],[['foo'],'bar']])
```

## Q16

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = ['foo',['bar'],'baz']
y = x[:]
y[1][:] = ['py']
print(x,x is y)
```

1. `['foo',['py'],'baz'] True`
2. `['foo',['py'],'baz'] False`
3. `['foo',[['py']],'baz'] True`
4. `['foo',[['py']],'baz'] False`

<div style="page-break-before:always"></div>

## Q17

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [[1],2,3]
y = x[:]
y = [4,x[0],y[0]]
x[0][0] = 3
print(y)
```

1. `[4,[1],[1]]`
2. `[4,[3],[1]]`
3. `[4,[1],[3]]`
4. `[4,[3],[3]]`

## Q18

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
import copy
x = [[[1]]]
y = copy.deepcopy(x)
print(x[0][0] is y[0][0],x[0][0][0] is y[0][0][0])
```

1. `True True`
2. `True False`
3. `False True`
4. `False False`

## Q19

次のPythonコードを実行した結果得られる出力を記述しなさい。解答例：`[[1],2,[3,4]]`

```python
x = [1,2,3]
x.append((4,3)*2)
print(x)
```

<div style="page-break-before:always"></div>

## Q20

次のPythonコードを実行したあと、変数yにリスト[8,5,2]を代入するためのコードとして正しいものを一つ選びなさい。

```python
x = list(range(10))
```

1. `y = x[-2:-9:-3]`
2. `y = x[2:9:-3]`
3. `y = x[-8:-1:-3]`
4. `y = x[-2:-8:-3]`

## Q21

次のPythonコードを実行した結果得られる出力を記述しなさい。解答例：`[[1],2,[3,4]]`

```python
x = [1]
x = [x+x]*2
x[0][0] = 3
print(x)
```

## Q22

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    elif i % 2 == 0:
        x -= 1
print(x)
```

## Q23

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    if i % 2 == 0:
        x -= 1
print(x)
```

<div style="page-break-before:always"></div>

## Q24

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
        if i % 2 == 0:
            x -= 1
print(x)
```

## Q25

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(5):
    for j in range(0,i):
        x += 1
    x -=1
print(x)
```

## Q26

次のPythonコードを実行したところ、下記の出力が得られたとします。

```python
import sys
x = sys.getsizeof("a")
y = sys.getsizeof("あ")
print(x,y)
```

```python
#出力
50 76
```

このとき、次のコードを実行したときの出力を整数値で答えなさい。

```python
print(sys.getsizeof("abcdefあ"))
```

<div style="page-break-before:always"></div>

## Q27

次のPythonコードを実行した際に得られる出力を文字列で答えなさい。解答例：`abCDefg`

```python
print("x".join("AkAaab".lower().split("aa")))
```

## Q28

次のPythonコードを実行した際に得られる出力を文字列で答えなさい。解答例：`abCDefg`

```python
text = "fgfgfgf"
print(text.replace("fg","f").replace("ff","g"))
```

## Q29

次のPythonコードを実行した結果出力として得られる文字列を答えなさい。解答例：`abCDefg`

```python
trans = {ord(c)-1:c for c in 'bef'}
print("abcdef".translate(trans))
```

## Q30

次のうち、Pythonのタプルであるものには○を、そうでないものには☓をつけなさい。(部分点あり)

1. `([],)`
2. `()`
3. `(,)`
4. `(0)`
5. `(([]))`

<div style="page-break-before:always"></div>

## Q31

次のPythonコードを実行したとします。そのあと、ファイル`output.txt`をテキストエディタで開くと、どのような文字列が書いてあるか、ひらがなで答えなさい。

```python
str_byte = bytes([0xe3,0x81,0x8b,0xe3,0x81,0x97,0xe3,0x81,0x93,0xe3,0x81,0x88])
with open('./output.txt','bw') as file:
    file.write(str_byte)
```

ただし、ひらがなの`utf-8`エンコーディングは次で与えられます。

```bash
あいうえお --> e38182 e38184 e38186 e38188 e3818a 
かきくけこ --> e3818b e3818d e3818f e38191 e38193 
さしすせそ --> e38195 e38197 e38199 e3819b e3819d 
たちつてと --> e3819f e381a1 e381a4 e381a6 e381a8 
なにぬねの --> e381aa e381ab e381ac e381ad e381ae 
はひふへほ --> e381af e381b2 e381b5 e381b8 e381bb 
まみむめも --> e381be e381bf e38280 e38281 e38282 
や　ゆ　よ --> e38284 e38080 e38286 e38080 e38288 
らりるれろ --> e38289 e3828a e3828b e3828c e3828d 
わ　　　を --> e3828f e38080 e38080 e38080 e38292 
ん　　　　 --> e38293 e38080 e38080 e38080 e38080 
```

## Q32

Python辞書を作成するコードとして正しいものには○を、誤っているものには☓をつけなさい。

1. `x = dict({'foo':1,'bar':2},baz=3)`
2. `x = {foo=1,bar=2,baz=3}`
3. `x = dict(zip('abc',(1,2,3)))`
4. `x = dict([('foo',1),('bar',2),('baz',3)])`
5. `x = dict(foo:1,bar:2,baz:3)`
6. `x = dict.fromkeys(set(('foo','bar','baz')),0)`

## Q33

次のPythonコードを実行した際に得られる出力を整数値で答えなさい。ただし64ビット処理系を仮定する。

```python
import sys
x = dict()
for i in range(0,5):
    x[i] = i
overhead = sys.getsizeof(dict()) - 128
print(sys.getsizeof(x)-overhead)
```

<div style="page-break-before:always"></div>

## Q34

次のPythonコードを実行したとします。

```python
x = dict()
x['cow']='mohmoh'
x['sheep']='mehmeh'
```

ただし、各文字列のハッシュ値は次の通りであるとします。

|文字列|ハッシュ値|
|--|--|
|'cow'|0x245810b898c00da1|
|'sheep'|0xbea68e2fc5c85f8a|
|'mohmoh'|0x81a17eca6daaa2a3|
|'mehmeh'|0xf8711f440a3f0962|

辞書`x`内部にあるインデックス配列の状態として正しいものを一つ選びなさい。

1. `1 2 -1 -1 -1 -1 -1 -1`
2. `0 1 -1 -1 -1 -1 -1 -1`
3. `-1 0 1 -1 -1 -1 -1 -1`
4. `-1 -1 1 0 -1 -1 -1 -1`

## Q35

次のPythonコードを実行したとします。

```python
x = {'dog','cat','horse'}
y = {'cow'}.union(x)
z = x.intersection({'cat','horse','sheep'})
```

次のうち、TrueになるものにはT、FalseになるものにはFと答えなさい。(部分点あり)

1. `z.issuperset(x)`
2. `x.issubset(y)`
3. `z.issubset(y)`
4. `z in y`

<div style="page-break-before:always"></div>

## Q36

次のPythonコードのうち、エラーが出ずに実行できるものには○を、そうでないものには☓をつけなさい。（部分点あり）

1. `{[],()}`
2. `{{(0)}}`
3. `{'':[]}`
4. `{():dict()}`
5. `{([],):1}`
6. `dict(5='a')`

## Q37

次のPythonコードを実行した際に出力される整数を書きなさい。

```python
print({i % 4:i for i in range(10)}[0])
```

## Q38

次のコードを実行したとき、`x`には何が代入されているか答えなさい。

```python
def func(x):
  if x > 1:
    return
  return x

x = func(2)
```

## Q39

次のPythonコードを実行した際に、`x`に格納されているリストを記述しなさい。例:`[1,2,3,4]`

```python
def generator():
  x = 1
  for i in range(2,7):
    yield x
    x *= i

gen = generator()

x = list(gen)
```

<div style="page-break-before:always"></div>

## Q40

次のPythonコードを実行した際に出力される整数を答えなさい。

```python
x = range(10)
y = [i if i%2==0 else -i for i in x if i % 3 != 0]
print(y[3])
```

## Q41

次のPythonコードは100以下の全ての素数を出力するためのコードです。(a)-(c)に当てはまるコードを1~4から選びなさい。

```python
for i in range(2,100):
  for j in range(2,i):
    (a)______
      (b)_____
  else:
    (c)______
```

1. `print(i)`
2. `break`
3. `continue`
4. `if i % j == 0`

<div style="page-break-before:always"></div>

## Q42

次のPythonコードは、"My teacher is a crazy guy."という文字列に含まれる各アルファベットの出現回数を印字するものである(大文字と小文字は区別しない)。

```python
string = 'My teacher is a crazy guy.'
trans_rule = {' ':'','.':''}
trans = str.maketrans(trans_rule)
sclean = string.lower().translate(trans)
x = dict()
for c in (a)_____:
  if c in (b)_____:
    x[c] += 1
  else:
    x[c] = 1
for k in sorted(x):
  print("{}/{}".format(k,x[k]))
```

出力は次のようになります。

```bash
a/3
c/2
e/2
g/1
h/1
i/1
m/1
r/2
s/1
t/1
u/1
y/3
z/1
```

(a)-(b)に当てはまる正しいコードを次から選びなさい。

1. `x.items()`
2. `sclean`
3. `set(sclean)`
4. `x.keys()`
