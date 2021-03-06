# Numbers API handling the v2.1 SOAP-API of NMBRS


## Installation

    $ gem install numbers_api


## Example Usage

  Initialize a configuration object:

    $ config = NumbersApi::Configuration.new("user@email.com", "nmbrs_api_key_example123", "numbers_company_id (optional)")

  Initialize a service (company_service, debtor_service or employee_service)

    $ company_service = NumbersApi::CompanyService.new(config)

  Make a request to the service

    $ company_service.request(:list_get_all)

  Optionally you can pass in extra parameters, for example:

    $ company_service.request(:cost_center_get_list, company_id: 37727)


### For a list of available methods:

  Check lib/numbers_api/company_service.rb / debtor_service.rb / employee_service.rb



### Api documentation

  https://support.nmbrs.nl/hc/nl/sections/200668406-Nmbrs-API-v2-1-Latest-Reference