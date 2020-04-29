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
 
# Requirements for cd4pe
mod 'puppetlabs-hocon', '1.0.1'
mod 'puppetlabs-puppet_authorization', '0.5.0'
mod 'puppetlabs-stdlib', '4.25.1'
mod 'puppetlabs-docker', '3.2.0'
mod 'puppetlabs-reboot', '2.0.0'
mod 'puppetlabs-powershell', '2.2.0'
mod 'puppetlabs-apt', '6.2.1'
mod 'puppetlabs-translate', '1.1.0'

mod 'concat',
  :git => 'git@github.com:elainemccloskey/puppetlabs-concat.git',
  :tag => 'v5.2.1'
