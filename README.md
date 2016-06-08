# PivotalTrackerPr
- `PivotalTracker`のストリーIDとストリー名を取得し、カレントブランチの`PullRequest`を作成する

## Installation

```ruby
$ gem install pivotal_tracker_pr
```

## Usage
- 下記の環境変数を設定しておく
  - `PT_TOKEN`：`PivotalTracker`のアクセストークン
  - `PT_PROJECT_ID`：`PivotalTracker`のプロジェクトID
- ブランチを作成するとき、`PivotalTracker`のストリーIDを含めるように命名する
- `git commit; git push`の後、`PullRequest`を作ろうとするタイミングで、`pivotal_tracker_pr create`を実行する

## TODO
- [ ] PullRequestのテンプレートをERBに切り出す
- [ ] ストリーIDのパラメータを受け取る

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment. Run `bundle exec pivotal_tracker_pr` to use the gem in this directory, ignoring other installed copies of this gem.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/blueplanet/pivotal_tracker_pr.