---
layout: post
title:
date: 2020-05-18 10:45:38 -7000
tags: rails react
categories: todo-app
---

# To do App - react and rails

- I am following these tutorials
- [Ruby on Rails with React Tutorial](https://stevepolito.design/blog/rails-react-tutorial/)
- [How To Set Up a Ruby on Rails Project with a React Frontend](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-ruby-on-rails-project-with-a-react-frontend)

# Devise - hiding the secret key

- Key wasn't hidden by default so I used it as a test of reverting commits
- https://gist.github.com/CrookedNumber/8964442
- https://superuser.com/questions/926915/how-can-i-delete-old-commits-in-github-via-terminal
- https://devconnected.com/how-to-remove-files-from-git-commit/
- http://www-cs-students.stanford.edu/~blynn/gitmagic/ch05.html#_8230_and_then_some

## Steps i ended with

`git reset --soft <commit-number>`

- To uncommit all the files up to the one you want to change
- change the file you want, it kind of flattens all the commit up to the one you want
  `git commit`
  `git push origin -f`

  - I hid it through using the method I used in the minimal twitter app and that worked.

# Devise creating views

- `rails generate devise:views`
- This sets up all the views for logging in etc

# seeding data and avoiding duplicates

- `rake db:reset` to wipe db if you have duplicates and only seeded data
- Use `find_or_create_by` instead of just `create`
- [avoiding duplicates created via seeds.rb](https://stackoverflow.com/questions/31758576/avoid-duplicate-records-created-via-seeds-rb)

# creating jbuilder files for controller actions

# trying to use postman

- Need to set up a user auth token to use postman. Needs further investigation
