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

