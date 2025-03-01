# E-Commerce-Store-for-Handmade-Goods

/（网站根目录）
├─ index.php              # 主页
├─ config.php             # 数据库配置和全局初始化
├─ .htaccess              # （可选）URL 重写规则
├─ assets/                # 静态资源和上传文件
│   └─ avatars/           # 用户头像上传目录
├─ auth/                  # 用户身份认证相关页面
│   ├─ register.php       # 用户注册（带邮箱验证 & reCAPTCHA）
│   ├─ login.php          # 用户登录
│   ├─ logout.php         # 用户注销
│   ├─ activate.php       # 邮件激活账户
│   └─ profile.php        # 个人资料管理（用户名、邮箱、密码、头像修改）
├─ products/              # 商品浏览相关页面
│   ├─ product_list.php   # 商品列表页
│   └─ product_detail.php # 商品详情页
├─ checkout/              # 结账相关页面
│   ├─ checkout.php       # 购物车 & 结账页面（地址管理 & PayPal 支付）
│   └─ place_order.php    # 处理订单提交（创建订单并跳转至支付）
├─ orders/                # 订单查看页面
│   ├─ order_list.php     # 用户订单历史（分页）
│   └─ order_detail.php   # 订单详情查看
├─ admin/                 # 管理员后台
│   ├─ admin_dashboard.php# 管理员仪表盘
│   ├─ admin_users.php    # 用户管理（按用户名/邮箱搜索，启用/禁用用户）
│   └─ admin_user_toggle.php # 执行启用/禁用用户操作
└─ payments/              # 支付相关处理
    ├─ paypal_success.php # 支付成功返回页面
    └─ paypal_ipn.php     # PayPal IPN通知处理接口