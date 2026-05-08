# 仕様

        ## 対象レコード

        - `studyTimer`
- `reviewQueue`
- `mockExam`
- `resultMemo`

        ## 必須項目

        `title`, `duration`, `nextAction`

        ## 警告項目

        `reviewDate`, `weaknessTag`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        学習ログはブラウザ内保存だけにし、ログインや外部送信を行わない
