Git Pull Request 流程
=
概論
-
　　要讓其他人參與一個專案的開發，最平常的方法就是將該成員加入到該專案的協同開發名單內。但是只要是協同開發成員，就可以自由地對專案執行 Pull 與 Push 等動作，故想要對不同工作性質和權限的成員做約束，就要有效地運用 Git 的各式功能，管制哪些人可以直接控制專案。

　　Pull Request 在字面上的意思是請求對方將這個變更拉過去，意即需要對方（專案的擁有者）同意後，才將此變更記錄到 Git 上。在這之前，要將專案 Fork 到自己的帳號下。Fork 的字面上指的是叉子，可以想像成將對方的專案用叉子叉到自己這邊。

　　之後將專案 Clone 到自己的電腦上，就像平時一樣進行編寫。完成後將專案 commit 並 push 到自己的帳號。

　　最後要將變更傳回原本的地方（對方的版本）時，則使用 pull request 發出通知。待對方同意後，將變更 merge （合併）到原先的版本，即完成整個程序。
實作過程
-
![enter image description here](http://i.imgur.com/5r4XWS5.jpg)
	　　假設 Vic（對方）有一專案要交給 Dispy（自己）開發，但是 Vic 想要事先檢查 Dispy 編寫的內容，避免 Push（推送）有問題的變更，造成專案開發的困難。故 Vic 告知該專案的位置，讓 Dispy 使用 Fork 功能到自己的帳戶。
	　　之後 Dispy Checkout 專案，開始進行工作。完成後將變更上傳到自己號戶下的 Repository（倉庫）。在 GitHub 專案頁面上按 New Pull Respository 按鈕，將修改通知傳給 Vic，即專案原本的擁有者。
備註
-
 - Pull Request 通常會與 Fork 一起談，因為是將專案 Fork 過來，最後再 Pull Request 回去。
 - 此作業流程大多是在 GitHub （或其他 Git 系統）網站操作。 只能在同一個 Git 系統操作（GitHub 專案只能 Fork 到
 - GitHub 帳號，不能到 BitBucket 帳號。至少目前沒試過能 Fork 到不同 Git 系統的方法）。

> Written with [StackEdit](https://stackedit.io/).