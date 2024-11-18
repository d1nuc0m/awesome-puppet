# Awesome Puppet [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

An (opinionated) awesome list of resources about Puppet, a configuration
management software.

It has been inspired by [rnelson0's list](https://github.com/rnelson0/awesome-puppet) and its forks, but it is not a fork of that list due to the lack of a license.

**Disclaimer**: Puppet is a trademark of Puppet, Inc., Perforce Software, Inc. or an affiliate ([link](https://www.puppet.com/docs/puppet/8/copyright-trademark)).
This project is not representing these companies, nor is in any way endorsed by them. All other trademarks mentioned in this project are property of their respective owners.

## Contents <!-- omit in toc -->
- [Books](#books)
- [IDE tools](#ide-tools)
- [Learning](#learning)
- [Modules](#modules)
  - [Modules Development](#modules-development)
  - [Modules Management](#modules-management)
- [Puppet Tools](#puppet-tools)
  - [Linters, Testers, Validators](#linters-testers-validators)

## Books

- [Puppet 8 for DevOps Engineers](https://www.packtpub.com/en-us/product/puppet-8-for-devops-engineers-9781803231709) - Probably the most up-to-date book about Puppet, focusing on the use of Puppet 8.
- [Puppet Best Practices](https://www.oreilly.com/library/view/puppet-best-practices/9781491922996/) - Written for Puppet 6, it's still a valid resource for Puppet 7/8 due to the focus on best practices and changes between these majors being mostly behind the scenes.

## IDE tools

- RubyMine and other JetBrains IDEs
    - [Puppet Plugin for JetBrains IDEs](https://plugins.jetbrains.com/plugin/7180-puppet) - Provides formatting, highlighting, assistance and more for Puppet >= 3.x.
- Vim
    - [vim-puppet](https://github.com/rodjek/vim-puppet) - Adds automatic alignment, formatting and highlighting for Puppet.
- Visual Studio Code\Codium and Theia IDE
    - [Puppet VSCode extension](https://puppet-vscode.github.io/) - Available in [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=puppet.puppet-vscode) and [Open VSX Registry](https://open-vsx.org/extension/puppet/puppet-vscode).
    Provides formatting, Intellisense, linting and more.

## Learning

- Hiera
    - hiera-eyaml
      - [Hiera-Eyaml: How to Use It - _Puppet Blog_](https://www.puppet.com/blog/puppet-eyaml-hiera-data) - Quick introduction to hiera-eyaml.
      - [HOWTO Set Up and Utilize hiera-eyaml - _SIMP docs_](https://simp.readthedocs.io/en/master/HOWTO/20_Puppet/Hiera_eyaml.html) - Step-by-step introduction to hiera-eyaml.
- [Puppet Cookbook](https://www.puppetcookbook.com) - Cookbook of example solutions in Puppet for different tasks.
- [PuppetModule.info](https://www.puppetmodule.info/) - Community-maintained module documentation website.
    - [Source](https://github.com/voxpupuli/puppetmodule.info) - Available on GitHub.
- r10k
    - [Fattening the workflow, part 2: r10k - _Puppeteers blog_](https://www.puppeteers.net/blog/fattening-the-workflow-part-2-r10k/) - Quickstart on r10k.
    - [Managing code with r10k - _Puppet Enterprise docs_](https://www.puppet.com/docs/pe/latest/r10k) - PE docs, but r10k can be used with Open Source Puppet.
- [Vox Pupuli](https://voxpupuli.org/) - Open Source community for Puppet modules, tools and docs authors.
    - [Plugins list](https://voxpupuli.org/plugins/) - Plugins, tools and resources for Puppet, practically an awesome list.

## Modules

- [puppet-collections](https://github.com/voxpupuli/puppet-collections) - Iterator written in Puppet.
- [puppet-example](https://github.com/voxpupuli/puppet-example) - Example repository for Puppet modules automation and development.
- [puppet-extlib](https://github.com/voxpupuli/puppet-extlib) - Extension of the [Standard Library](https://github.com/puppetlabs/puppetlabs-stdlib).
- [puppet-healthcheck](https://github.com/voxpupuli/puppet-healthcheck) - Healthcheck resources.
- [puppet-puppet_certificate](https://github.com/voxpupuli/puppet-puppet_certificate) - Provider and resource for Puppet certificates.
- [puppetlabs-puppet_status_check](https://github.com/puppetlabs/puppetlabs-puppet_status_check) - Status checks for the Puppet infrastructure.

### Modules Development

- [metadata-json-lint](https://github.com/voxpupuli/metadata-json-lint) - Validator/linter for Puppet modules' metadata.json.
- [puppet-ghostbuster](https://github.com/voxpupuli/puppet-ghostbuster) - Helps to find unused code in Puppet.
- [Puppet Development Kit](https://www.puppet.com/docs/pdk/latest/pdk.html) - Collection of tools to develop, validate and test Puppet modules.

### Modules Management

- [g10k](https://github.com/xorpaul/g10k) - A r10k fork in Go.
- [Jens](https://github.com/cernops/jens) - Python toolkit to generate Puppet environments dynamically based on control repositories.
- [librarian-puppet](https://github.com/voxpupuli/librarian-puppet) - Bundler to manage Puppet modules through a Puppetfile, with support for dependencies defined in Modulefile or metadata.json.
- [ModuleSync](https://github.com/voxpupuli/modulesync) - Ruby gem to synchronize meta-files (Gemfile, .gitignore etc) between Puppet modules of an organization.
- [Pdksync](https://github.com/puppetlabs/pdksync) - Tool synchronize settings between multiple Puppet modules through PDK.
- [puppet-blacksmith](https://github.com/voxpupuli/puppet-blacksmith) - Ruby gem with Rake tasks to manage a module on the Puppet Forge.
- [r10k](https://github.com/puppetlabs/r10k) - Tool to manage git/SVN-based environments and modules defined in a [Puppetfile](https://github.com/puppetlabs/r10k/blob/main/doc/puppetfile.mkd), but [without dependency resolving](https://github.com/puppetlabs/r10k/issues/1031).
   - [puppet-r10k](https://github.com/voxpupuli/puppet-r10k) - Puppet module to manage r10k.
   - [ra10ke](https://github.com/voxpupuli/ra10ke) - Rake tasks for r10k and Puppetfiles.

## Puppet Tools

- [Beaker](https://github.com/voxpupuli/beaker) - Tool to run acceptance acceptance tests using VMs.
   - [beaker-hiera](https://github.com/voxpupuli/beaker-hiera) - Allows to use Hiera data in Beaker tests.
- [Hiera Data Manager](https://github.com/betadots/hdm) - Web interface to visualize/search Hiera data.
   - [puppet-hdm](https://github.com/voxpupuli/puppet-hdm) - Puppet module to install/manage Hiera Data Manager.
- [hiera-eyaml](https://github.com/voxpupuli/hiera-eyaml) - Hiera backend that allows to encrypt values in Hiera YAML files.
   - [hiera-eyaml-gpg](https://github.com/voxpupuli/hiera-eyaml-gpg) - Allows to use GPG encryption with hiera-eyaml.
- [Puppetboard](https://github.com/voxpupuli/puppetboard) - Web interface for PuppetDB that aims to be the equivalent of [Puppet Enterprise console](https://www.puppet.com/docs/pe/latest/console_accessing.html) for Open Source Puppet.
   - [puppet-puppetboard](https://github.com/voxpupuli/puppet-puppetboard) - Puppet module to install Puppetboard.
- [Puppet Bolt](https://www.puppet.com/docs/bolt/latest/bolt.html) - Agent-less orchestration tool, to run tasks/scripts/commands on remote nodes through SSH or WinRM.
   - [puppet-bolt](https://github.com/voxpupuli/puppet-bolt) - Puppet module to install/manage Bolt.
- [Puppet Catalog Diff](https://github.com/voxpupuli/puppet-catalog_diff) - Tool to compare Puppet catalogs.
- [Puppet Summary](https://github.com/skx/puppet-summary) - Web interface written in Go.
   - [puppet-puppet_summary](https://github.com/voxpupuli/puppet-puppet_summary) - Puppet module to install/manage Puppet Summary.
- [pypuppetdb](https://github.com/voxpupuli/pypuppetdb) - Python library to interact with the PuppetDB API.

### Linters, Testers, Validators

- [onceover](https://github.com/voxpupuli/onceover) - Run tests against a Puppet control repository (for example used with r10k).
- [puppet-syntax](https://github.com/voxpupuli/puppet-syntax) - Syntax checks for manifests, templates and Hiera YAML.
- [puppet-lint](https://github.com/puppetlabs/puppet-lint) - Test code against the Puppet style guide.
- [rspec-puppet](https://github.com/puppetlabs/rspec-puppet) - RSpec tests for Puppet manifests.

<!-- omit in toc -->
## Contributing

Contributions are welcome! [Guidelines are here](CONTRIBUTING.md).
