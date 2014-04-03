namespace :sass do
  desc "Build Sass file"
  task :build do
    sh 'sass ./sass/cornerstone.scss ./site/css/cornerstone.css'
  end
  
  desc "Watch Sass changes"
  task :watch do
    sh 'sass --watch ./sass/cornerstone.scss:./site/css/cornerstone.css'
  end
end

namespace :site do
  desc "Build Jekyll site"
  task :build do
    sh 'jekyll build --source ./site --destination ./site/_site'
  end
  
  desc "Serve Jekyll site"
  task :serve do
    sh 'jekyll serve --watch --source ./site --destination ./site/_site'
  end
  
  desc "Deploy Jekyll site to gh-pages branch"
  task :deploy do
    sh "git subtree push --prefix site origin gh-pages"
  end
end
