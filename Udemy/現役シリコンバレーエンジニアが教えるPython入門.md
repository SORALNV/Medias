## S3 Pythonの基本

Pythonは宣言しなくて良い。type(変数)でintやstrがわかる

int で定義後に文字代入で str 型への変更可能。
変数 = int(変数) で変更可能

int: 変数= 何か で指定して宣言も可能だが使わない。

変数の最初に数字はダメ

print('Hi','Mike',sep=aaa,end=bbb)
→HiaaaMikebbb     (sepで間のを、endで終わりを調整)

- 17 / 3
→ 5.6666666666667
- 17 // 3
→ 5
- 17 % 3
→ 2

- 5 ** 5
→ 3125

- round(pie,2)
→ 3.14

### math.メソッド名

print(heip(ライブラリやコマンド名))

print('I don't know')
→ ' のどこまでかがわからずにエラー
print('I don\'t know')で解決

print(r'C\name\name')
→ \n によって改行されるのを防ぐためにrawの略であるrをつける
print("""line1,line2,line3""")
→ 自動で改行されて出力される
print("""\line1,line2,line3\""")
→ 開業が前と後に入らない


変数に入れたものはと通常文字は＋で繋げないとprintできない
リテラル：’’で囲ったもの
可能: print('Hi''Mike') , print('Hi'+'Mike') , print('Hi'*3 + 'Mike')
不可能：c=asdfafd   print(c+'MIke')

s =( 'aaaaa','bbbbb')
s ='bbbb' \ 'aaaa'
で出力で一直線に並ぶ



### 文字列でもリストでも以下のように指定できる
word[?]
- -1 ラストの文字
- 0:2 0から2番目
- 2:5 2から5番目
- :2 最初から2番目
- 2; 2番目から最後まで
- :　全部

リストでできることは確定
- ::2 一個飛ばして
- ::-1 後ろから順に 


文字列のインデックスについて
word[0]= 'j'は不可能
word = 'j'+word[1:]なら可能

リストならそのまま置き換えが可能

s.　でメソッドを使用可能

### f-string

name = 'Jun'
family = 'Sakai'
print(f'My name is {name} {family}. Watashi ha {family} {name}')

### リストのメソッド
- list.append(100) 最後に100を追加
- list.insert(100)　最初に100を追加
- list.pop() 指定した要素をとってくる（下の文字列からは消える）（指定なしだと最後のものを取ってくる）
- del list[] で指定して要素を消せる
- list.remove(100) 100という要素を削除
- list.extend(list2) listにlist2を結合（list += list2 でも可能）
- list.index(a, b) aという数をb以降で探す

if 5 in list
→ listの中から5を探す


メモしすぎても仕方ないのでメモは最低限に


list []
tuple ()

tuple 新しい代入は不可能,indexやスライスなどのメソッドは使用可能。書き換えできないので読み込み専用。tuple内にリストを入れることは可能。カンマをつければ（）がなくてもタプルになる。
