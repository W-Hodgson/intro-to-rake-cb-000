namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  desc 'migrates changes to the database'
  task :migrate => :environment do
    Student.create_table
  end
end
