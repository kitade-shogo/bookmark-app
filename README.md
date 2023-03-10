# bookmark-app

ブックマーク管理アプリのリポジトリです

■ サービス概要
「後で読もう」とブックマークやリーディングリストに技術記事を登録するが、結局読まないままにしている人に
適切なタイミングで読む機会を提供する
「いつ」にフォーカスしたブックマーク管理・共有サービスです

■ サービス利用方法
①ユーザー登録・ログイン後、連携したChrome拡張機能を追加
②ブックマークに追加したいページへ移動後、インストールしたChrome拡張機能から重要度等の項目を選択して保存(ブックマーク登録)
③登録したブックマークはいつでもマイページのブックマークリストからご確認いただけます。
④登録時に選択された重要度に応じて、ブックマークしてから一定時間後に通知を送ります。


■ メインのターゲットユーザー
・プログラミング学習中の方
・学習コミュニティに参加中の方


■ ユーザーが抱える課題
1. 日々の学習やキャッチアップが大変なため、「後で読みたい」と感じる記事が多いのにも関わらず、忘れてしまって読む機会を失っている
2. 既存のブックマークマネージャには「いつ」ブックマークしたのかを直感的に理解できるUIが導入されていない
3. 他の人がどのような記事を参考にし、どのような記事を重要だと思っているかを知りたい


■ 解決方法
1. ブックマーク登録時に重要度も同時に登録。重要度別に一定時間後に通知する。（例: 重要度高 → 1日後に通知, 重要度低 → 1週間後に通知）
2. カレンダー機能を導入することにより、ブックマークした日時を視覚的に理解できるようにする。学習ログのような使い方も期待できる。
3. ユーザーのブックマークを集めた掲示板を作成する。また、重要度別にカテゴリ分けを行う。


■ 実装予定の機能（以下の例は実際のアプリの機能から一部省略しています）
<<MVPリリース>>
・ユーザー登録、削除機能
・ログイン、ログアウト機能
・ブックマーク機能(ブックマークしたいページへ移動後、Chrome拡張機能を通じてブックマークを保存することができる)
・カレンダー機能
・ブックマークリスト機能(自分がブックマークした記事のリスト)
・通知機能(LINEメッセージでの通知)

<<本リリース>>
・フォロー、フォロワー機能
・ブックマークリスト共有機能(フォローしているユーザー同士ではブックマークリストの閲覧が可能)
・掲示板機能(重要度別にユーザーがブックマークした記事を表示。全ユーザーが対象で、公開・非公開設定ができる)

■ なぜこのサービスを作りたいのか？
ブックマークした時には『後で読みたい』と思っていたのにそのまま忘れてしまうことがよくあり、せっかくの学習機会を捨てていて勿体無いと感じたからです。
また、ブックマークした時から時間が経っているほど、何を学習中にどういった理由でブックマークしたのか思い出しづらいので、適切なタイミングでリマインドしてくれるサービスが欲しいと思ったからです。


■ 主な使用技術 (予定)
フロントエンド: React, TypeScript
バックエンド: Ruby on Rails

■ スケジュール
企画〜技術調査：3/4 〆切
README〜ER 図作成：3/6 〆切
メイン機能実装：3/7 - 4/6
β 版を RUNTEQ 内リリース（MVP）：4/6 〆切
本番リリース：4/24