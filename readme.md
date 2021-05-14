### HOW TO DO
먼저, ruby, gem과 지킬을 설치 한 후 아래와 같이 install 한다.
```
gem install bundler jekyll minima jekyll-feed tzinfo-data rdiscount
```
로컬에서 작동해보기 위해서는 `_config.yml` 파일에서 아래의 코드 주석을 바꿔주어야 한다.
단, 다시 github로 올릴 때에는 remote로 설정해주어야 한다.
```
# theme: jekyll-theme-hydejack                # FOR LOCAL
remote_theme: hydecorp/hydejack@v9.0.0-rc.6   # FOR GITHUB (REMOTE)
```
그 다음, `_config.yml` 파일이 있는 경로에서 아래와 같이 커맨드를 실행하면 `127.0.0.1:4000` 에서 시행된다.
```
bundle install
bundle exec jekyll serve
```
<br>

### ADDITIONAL INFORMATION
- 새로운 페이지를 추가하기 위해서는 `_config.yml` 파일의 `menu` 부분에 추가할 페이지 이름을 추가를 해주어야 한다.
- 새로운 페이지는 markdown이나 html 어느 형태여도 상관 없다.
- 새로운 페이지를 추가할 때, 다른 페이지들과 마찬가지로 `layout`과 `sitemap`을 설정해주어야 한다.