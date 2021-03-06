---
layout: default
title: 設定について
---

# 管理画面にログインする

1.  まず WordPress に管理者アカウントでログインします。 http://example.com/wp-admin/

    ![管理画面]({{ site.baseurl }}/assets/images/7-1-001.png)

2.  左ペインの「設定」から「一般設定」をクリックします。

    ![設定]({{ site.baseurl }}/assets/images/7-1-002.png)

    # 一般設定

    ![一般設定]({{ site.baseurl }}/assets/images/7-1-003.png)

    ## サイトのタイトル

    このサイト全体のテーマを表わすタイトルをつけます。

    ## キャッチフレーズ

    このサイトを一言で説明します。

    ## WordPress アドレス (URL)

    WordPress をインストールした場所です。
    このアドレスを編集すると、サイトにアクセスできなくなる場合があります。
    編集する際は、[サイト URL の変更](http://wpdocs.osdn.jp/%E3%82%B5%E3%82%A4%E3%83%88_URL_%E3%81%AE%E5%A4%89%E6%9B%B4)をご覧ください。
    
    ## サイトアドレス (URL)

    読者が WordPress サイトにアクセスするためのアドレスです。
    サイトのホームページを 専用ディレクトリに配置にしたい場合、ここにアドレスを入力します。
    詳しくは、[WordPress を専用ディレクトリに配置する](https://wpdocs.osdn.jp/WordPress_%E3%82%92%E5%B0%82%E7%94%A8%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E3%81%AB%E9%85%8D%E7%BD%AE%E3%81%99%E3%82%8B)をご覧ください。

    ![一般設定]({{ site.baseurl }}/assets/images/7-1-004.png)

    ## メールアドレス

    サイト管理のためのメールアドレスを指定します。WordPress のバージョンアップや新規ユーザーの通知などが届きます。

    ## メンバーシップ

    だれでもユーザー登録ができるようにしたいとき、ここにチェックをいれます。

    ## 新規ユーザーのデフォルト権限グループ

    ドロップダウンボックスで、新規ユーザーに割り当てるデフォルトの役割を選択します。(役割によって与えられる権限が異なります。)
    このデフォルトの役割は、新規に登録したメンバー、もしくは管理画面 > ユーザー > ユーザー画面経由で加えられたユーザーに割り当てられます。選択できるのは、権限が大きい順に「管理者」「編集者」「投稿者」「寄稿者」「購読者」の5種類です。

    ## タイムゾーン

    あなたが活動している地域とタイムゾーンが一致する都市を選択します。

    ![一般設定]({{ site.baseurl }}/assets/images/7-1-005.png)

    ## 日付のフォーマット

    年月日の表示方法を選択します。
    デフォルトでは「○年○月○日」のようなフォーマットになっています。
    使用したいフォーマットを選択します。

    ## 時刻フォーマット

    「時刻フォーマット」は時と分の表示方法を選択します。

    ## 日付と時刻の書式の解説

    WordPress の関数の中には、the_date() や the_time() などのように投稿日時を表示させるものがあります。
    こういった関数の中にはフォーマット文字列という、日時の表示方法を決める引数を使うことができます。
    フォーマット文字列は日付関係の色々なパーツを組み合わせることができます。

    ## 週の始まり

    WordPress カレンダーに設定したい週の始まりをドロップダウンボックスから選択します。
    標準の設定は「月曜日」で、毎月のカレンダーで週の最初に月曜日が表示されます。カレンダーで週が日曜日から始まるようにするには、ドロップダウンボックスから「日曜日」を選択します。

    ## サイトの言語

    WordPress 管理画面の言語を選択します。

3.  左ペインの「設定」から「表示設定」をクリックします。

    # 表示設定

    この表示設定画面の設定項目は、数は少ないけれど重要なものです。
    サイトのフロントページ（メインページ）の表示を投稿と「静的」ページのどちらにするかを決められます。
    また、メインページに表示する投稿数も調節できます。
    さらに、フィード配信機能について、自分のサイトから読者のウェブブラウザやフィードリーダーなどのソフトウェアにどのような情報を配信するかを決められます。
    
    # パーマリンクの設定

    「サイトアドレス(URL)」に続けるパーマリンクやアーカイブの URL 構造を設定することができます。  
    URL をカスタマイズすることで、リンクの美しさや使いやすさを改善できます。

    ## 共通設定
    
    ### 基本

    投稿した記事のIDをURL構造に利用します。  
    WordPressをインストールした時点では、基本が選択された状態になります。  
    (例) `http://example.com/?p=123`

    ### 日付と投稿名

    投稿した日付とタイトルをURL構造に利用します。  
    (例) `http://example.com/2017/09/17/sample-post/`
    
    ### 月と投稿名
    
    投稿した月とタイトルをURL構造に利用します。  
    (例) `http://exaple.com/2017/09/sample-post/`
    
    ### 数字ベース
    
    投稿した記事のIDをURL構造に利用します。  
    「基本」との違いは、URL構造に `/archives/` を用いる点です。  
    (例) `http://example.com/archives/123`
    
    ### 投稿名
    
    投稿した記事のタイトルをURL構造に利用します。  
    (例) `http://example.com/sample-post/`
    
    ### カスタム構造

    以上の項目以外にも、任意でURL構造を設定することができます。  
    利用できる構造タグは、WordPress 日本語版 codex内、「[パーマリンクの使い方](https://wpdocs.osdn.jp/%E3%83%91%E3%83%BC%E3%83%9E%E3%83%AA%E3%83%B3%E3%82%AF%E3%81%AE%E4%BD%BF%E3%81%84%E6%96%B9)」にある「構造タグ」の説明を参照してください。

    ## オプション
    
    カテゴリー・タグの URL 構造をカスタマイズすることもできます。デフォルトのままにしたければ空欄にしてください。  
    利用できる構造タグは、WordPress 日本語版 codex内、「[パーマリンクの使い方](https://wpdocs.osdn.jp/%E3%83%91%E3%83%BC%E3%83%9E%E3%83%AA%E3%83%B3%E3%82%AF%E3%81%AE%E4%BD%BF%E3%81%84%E6%96%B9)」にある「構造タグ」の説明を参照してください。
    
    ### カテゴリーベース
    
    カテゴリのURL構造を設定することができます。  
    空欄の場合、 `/category/` が指定されます。

    ### タグベース
    
    タグのURL構造を設定することができます。  
    空欄の場合、 `/tag/` が指定されます。