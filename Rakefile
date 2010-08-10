require 'rubygems'
gem 'hoe', '>= 2.1.0'
require 'hoe'
require 'fileutils'
require './lib/eudict-gem'

Hoe.plugin :newgem

$hoe = Hoe.spec 'eudict-translate' do
  self.developer 'BKrsta', 'bkrsta@gmail.com'
  self.rubyforge_name = 'eudict-translate'
  self.extra_deps = [
    ['mechanize','> 0'],
    ['hpricot','> 0'],
    ['terminal-table','> 0']
  ]
end

require 'newgem/tasks'
Dir['tasks/**/*.rake'].each { |t| load t }
