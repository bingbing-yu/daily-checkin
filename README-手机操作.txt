【我的每日打卡｜云端同步 PWA】

文件：
- index.html：网页主体
- manifest.json：安装到手机/平板桌面的 PWA 配置
- service-worker.js：离线缓存
- icon-192.png / icon-512.png：桌面图标

下一步需要：
1. 建 Supabase 项目和 daily_records 表，并开启 RLS（按说明执行 SQL）。
2. 把这 5 个文件发布到 HTTPS 网站，例如 GitHub Pages。
3. 用 Edge/Chrome 打开网址，在网页里填 Supabase Project URL 和 anon public key。
4. 注册一个账号。
5. 手机和平板都打开同一个网址，用同一个账号登录，即可同步。

绝对不要把 Supabase service_role key 放进网页。
