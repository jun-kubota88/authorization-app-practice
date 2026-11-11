## 概要
COACHTECH 教材 Tutorial 10-3「認可機能 ハンズオン演習」で作成した成果物です。

## 使用技術
- PHP 8.x
- Laravel 10.x
- Policy / Gate（認可）
- Laravel Fortify（認証）

## 学んだこと
- 認証（誰か）と認可（何ができるか）の違いと使い分け
- Policy クラスでモデルに紐づく認可ロジックを定義する仕組み
- Blade の @can ディレクティブとコントローラの $this->authorize()

## 動作確認
- ローカルホストにアクセスし、Web画面にて表示されることを確認しました。
ユーザーAでログイン時の投稿一覧（ユーザーAの投稿にのみ「編集」「削除」ボタンが表示される）
  <img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/fe449abd-7329-42fe-b988-9f3f0c50f0a6" />
ユーザーBでログイン時の投稿一覧（ユーザーBの投稿にのみ「編集」「削除」ボタンが表示される）
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f2f12b0f-df2d-4248-911b-1ce41402e099" />
他人の投稿を直接編集しようとした場合（403 Forbiddenエラーが表示される）
<img width="1920" height="1128" alt="image" src="https://github.com/user-attachments/assets/7e506f1b-5bc8-4d47-9d52-18e5877f2f0a" />


