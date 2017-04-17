# mentoring_exam_for_new_mentors

こちらのファイルは、仮メンター/新メンター向け模擬質問研修の進め方についてのナレッジです。

# 目次
+ こちらのドキュメントでわかること
+ ディレクトリ構成
+ 模擬質問研修の進め方
+ 模擬質問の各問題の概要/解答

# こちらのドキュメントでわかること
+ ディレクトリ
+ 模擬質問研修の進め方について
+ 模擬質問の各問題の概要/解答


# こちらのディレクトリについての説明

こちらのディレクトリに含まれている「Lesson2」 ~ 「Lesson4」はそれぞれwebアプリケーションカリキュラムに対応しています。

# 模擬質問問題の概要/解答

## Lesson2

### question1.rb

#### 問題概要
Lesson2、レビューアプリにおいてのタイポの問題


#### 使用方法
1. ターミナルからquestion1.rbを実行
2. Lesson2のレビューアプリの実行操作を行う
3. 最後まで実行すると、最後の出力でreviewが表示されない


#### 解答



#### 元コード

```
  # メソッドの定義
  def post_review
    # 変数の定義
    post = {}
    puts "ジャンルを入力してください："
    post[:genre]  = gets.chomp
    puts "タイトルを入力してください："
    post[:title]  = gets.chomp
    puts "感想を入力してください："
    post[:riview] = gets.chomp
    line   = "---------------------------"

    # レビューの描画
    puts "ジャンル : #{post[:genre]}\n#{line}"
    puts "タイトル : #{post[:title]}\n#{line}"
    puts "感想 :\n#{post[:review]}\n#{line}"
  end

  def read_reviews
    # レビューを読む
  end

  def end_program
    # プログラムを終了する
  end

  def exception
    puts "入力された値は無効な値です"
  end

  # メニューの表示
  puts "レビュー数：0"
  puts "[0]レビューを書く"
  puts "[1]レビューを読む"
  puts "[2]アプリを終了する"
  input = gets.to_i

  if input == 0 then
    post_review         # post_reviewメソッドの呼び出し
  elsif input == 1 then
    read_reviews        # read_reviewsメソッドの呼び出し
  elsif input == 2 then
    end_program         # end_programメソッドの呼び出し
  else
    exception           # exceptionメソッドの呼び出し
  end
```

### question2.rb

#### 問題概要
体験カリキュラム、代入の = が1本になってしまっている問題


#### 使用方法
1. ターミナルからquestion2.rbを実行
2. 毎回「あいこ」になってしまい、勝ち、負けの判定ができない


#### 解答


#### 元コード

```
  puts "最初はグーじゃんけん..."
  puts "[0]:グー\n[1]:チョキ\n[2]:パー"

  player_hand = gets.to_i
  cpu_hand = rand(3)

  if player_hand = cpu_hand
    puts "あいこです！"
  elsif (player_hand == 0 && cpu_hand == 1) || 
        (player_hand == 1 && cpu_hand == 2) || 
        (player_hand == 2 && cpu_hand == 0)
    puts "あなたの勝ちです！"
  else
    puts "あなたの負けです！"
  end
```

## Lesson3

### question1.html/question1.css

#### 問題概要
Lesson3、htmlに全角スペースが入っていることにより余計な空白ができてしまう問題


#### 使用方法
1. question1.htmlをブラウザにて開く


#### 解答


### question2.html/question2.css

#### 問題概要
HTML問題にて、clearfixについての質問

####質問内容
html/css問題2にて、模範解答どおりでなくclearfixを利用して解こうとしたがうまくいかなかった。
なぜか？また、claerfixを利用して解くとしたら、どのように書けるか？


#### 使用方法
1. question2.htmlをブラウザにて開く


#### 解答


