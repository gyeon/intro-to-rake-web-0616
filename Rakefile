desc 'outputs hello to the terminal'
namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end

desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

desc 'migrate changes to database'
namespace :db do 
  task :migrate => :environment do
    Student.create_table
  end
end

task :environment do
  require_relative './config/environment'
end

desc 'seeds the database with dummy data'
namespace :db do
  task :seed do
    require_relative './db/seeds.rb'
  end
end