# Senju

Multi issue management serivces integration platform (CLI)

* Github
* GitLab
* Trello

## Installation

    $ gem install senju

## Configuration

Making `~/.senju` directory.

    $ mkdir ~/.senju

### Credentials

Edit `~/.senju/credentials`.

```
<type>: <access token>
```

### Projects

Edit `~/.senju/projects`.

```
<project name>:
  repo: <team/repository>
  type: <repository type>
```

or interactively `$ senju add <name>`.

## Usage

All repository issues.

    $ senju

Repository issues.

    $ senju <repository alias> [issues]

Repository Pull-Requests.

    $ senju <repository alias> pr

Issue/Pull-Request detail.

    $ senju <repository alias> <issue no> [-v|comments|diff]

Merge Request detail (GitLab)

    $ senju <repository alias> mr <issue no> [-v|comments|diff]

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/senju.
