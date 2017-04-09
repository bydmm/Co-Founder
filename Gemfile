source 'http://gems.ruby-china.org'

# 使用 github: 'rails/rails' 这样的方法引入中间件
git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

# 核心组件
gem 'rails', '~> 5.0.2' # 最新
gem 'puma', '~> 3.0' # 高速Webserver，但是建议部署在Nginx的反向代理之后
gem 'bcrypt', '~> 3.1' # 慢哈希加密

# 数据库相关
gem 'pg', '0.18.1' # 使用PostgreSQL，和Mysql说拜拜
gem 'redis', '~> 3.0' # 可持久化的键值对数据库

# 生产环境部署相关
gem 'figaro', '~> 1.1' # 管理环境变量

# 任务队列
gem 'sinatra', :require => nil  # for sidekiq web in routes
gem 'sidekiq'
gem 'sidekiq-failures'

# 前端构建, Rails的前端构建工具还是够用的
gem 'sass-rails', '~> 5.0'  # Rails Sass支持
gem 'uglifier', '>= 1.3.0' # 混淆JS
gem 'coffee-rails', '~> 4.2' # Rails Coffee支持
gem 'jquery-rails' # 引入jQuery

# 开发和测试用的
group :development, :test do
  gem 'listen'
  gem 'pry-rails'
  gem 'pry-byebug'
end
