【我的每日打卡·完整云端同步版】

这次是完整修正版，重点修复：
1. 今日打卡项目必须完整显示；
2. 月度日历完整显示当月所有日期；
3. 月份可用左右按钮切换；
4. 三项关键目标的日历图标规则：
   - 三项全部完成：🙂
   - 没完成戒烟：🚬
   - 没按计划早睡：💤
   - 有手淫/未完成：🧻
   - 多项失败时同时显示对应图标，不显示🙂；
   - 尚未有任何记录的日期不显示失败图标；
5. 保留六项习惯、心情、备注、统计、连续戒烟、JSON备份；
6. 保留 Supabase 登录、注册、云端同步；
7. 修复上一版 JavaScript 语法错误；
8. 更新 Service Worker 缓存版本，避免旧网页缓存继续生效。

【GitHub 替换方法】
最稳妥的方法：把这个文件夹里的 5 个文件全部替换到 daily-checkin 仓库根目录：
- index.html
- service-worker.js
- manifest.json
- icon-192.png
- icon-512.png

如果 GitHub 里已经有同名文件，就逐个打开后删除/替换，再提交修改。

【Supabase】
Project URL 已预填：
https://adoocohumgvxnlngxdwr.supabase.co

网页第一次打开后，在“云端同步”填写：
- Project URL
- Publishable key（或旧版 anon public key）

不要填写 Service Role / Secret key。

不需要重新创建 daily_records 表，也不要删除现有表和 RLS 政策。
