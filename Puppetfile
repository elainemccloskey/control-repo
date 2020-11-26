def default_branch(default)
  begin
    match = /(.+)_(cdpe|cdpe_ia)_\d+$/.match(@librarian.environment.name)
    match ? match[1]:default
  rescue
    default
  end
end
 
forge 'https://forge.puppet.com'
 
mod 'puppetlabs-cd4pe', :latest
mod 'm0dular-crl_truncate', '0.1.0'
 
# Requirements for cd4pe
mod 'puppetlabs-hocon', '1.0.1'
mod 'puppetlabs-puppet_authorization', '0.5.0'
mod 'puppetlabs-docker', '3.2.0'
mod 'puppetlabs-reboot', '2.0.0'
mod 'puppetlabs-powershell', '2.2.0'
mod 'puppetlabs-apt', '6.2.1'
mod 'puppetlabs-translate', '1.1.0'
mod 'puppetlabs-comply', '0.9.0'

# dependencies for comply
mod 'puppet-archive', '4.4.0'
mod 'puppetlabs-chocolatey', '5.0.2'
mod 'puppetlabs-inifile', '4.2.0'
mod 'puppetlabs-java', '6.3.0'
mod 'puppetlabs-ruby_task_helper', '0.4.0'
mod 'puppetlabs-stdlib', '6.3.0'

mod 'concat',
  :git => 'git@github.com:elainemccloskey/puppetlabs-concat.git',
  :tag => 'v5.2.1'
