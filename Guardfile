# Guardfile. More info at https://github.com/guard/guard#readme
# required gems: guard, guard-haml, guard-sass, guard-coffeescript

guard 'haml', :output => 'public', :input => 'src/templates', :haml_options => { :ugly => true } do
    watch %r{^src/.+(\.haml)}
end
guard 'sass', :input => 'src/css', :output => 'public/css', :all_on_start => true, :extension => '.css'    
guard 'coffeescript', :input => 'src', :output => 'public', :all_on_start => true
guard :copy, :from => 'src/img', :to => 'public'
guard :copy, :from => 'src/js/libs', :to => 'public/js/libs', :mkpath => true

# Sample guardfile block for Guard::Haml
# You can use some options to change guard-haml configuration
# :output => 'public'                   set output directory for compiled files
# :input => 'src'                       set input directory with haml files
# :run_at_start => true                 compile files when guard starts
# :notifications => true                send notifictions to Growl/libnotify/Notifu
# :haml_options => { :ugly => true }    pass options to the Haml engine

#guard 'haml' do
#  watch(/^.+(\.html\.haml)/)
#end
