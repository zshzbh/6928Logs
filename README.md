# 6928 Logs

Issue 6928 full log



# CLI
```

~ $ aws --region us-east-1 logs start-query   --log-group-name '/aws/lambda/6896'   --query-string "filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\d+) MB\sMax Memory Used: (?<memoryUsed>\d+) MB/"   --start-time 1742205559 --end-time 1742248759 --debug
```
# CLI full log 
```
2025-03-18 19:18:21,448 - MainThread - awscli.clidriver - DEBUG - CLI version: aws-cli/2.24.21 Python/3.12.9 Linux/6.1.127-135.201.amzn2023.x86_64 exec-env/CloudShell exe/x86_64.amzn.2023
2025-03-18 19:18:21,448 - MainThread - awscli.clidriver - DEBUG - Arguments entered to CLI: ['--region', 'us-east-1', 'logs', 'start-query', '--log-group-name', '/aws/lambda/6896', '--query-string', "filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\\d+) MB\\sMax Memory Used: (?<memoryUsed>\\d+) MB/", '--start-time', '1742205559', '--end-time', '1742248759', '--debug']
2025-03-18 19:18:21,465 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function add_s3 at 0x7f8a36a3bb00>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function add_ddb at 0x7f8a36c5dd00>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <bound method BasicCommand.add_command of <class 'awscli.customizations.configure.configure.ConfigureCommand'>>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function change_name at 0x7f8a36db2fc0>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function change_name at 0x7f8a36dd44a0>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function alias_opsworks_cm at 0x7f8a36a4a3e0>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function add_history_commands at 0x7f8a36cb49a0>
2025-03-18 19:18:21,466 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <bound method BasicCommand.add_command of <class 'awscli.customizations.devcommands.CLIDevCommand'>>
2025-03-18 19:18:21,469 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <function add_waiters at 0x7f8a36a4a2a0>
2025-03-18 19:18:21,469 - MainThread - botocore.hooks - DEBUG - Event building-command-table.main: calling handler <bound method AliasSubCommandInjector.on_building_command_table of <awscli.alias.AliasSubCommandInjector object at 0x7f8a36b02180>>
2025-03-18 19:18:21,469 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/data/cli.json
2025-03-18 19:18:21,474 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <function resolve_types at 0x7f8a36b6ad40>
2025-03-18 19:18:21,474 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <function no_sign_request at 0x7f8a36b6b060>
2025-03-18 19:18:21,474 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <function resolve_verify_ssl at 0x7f8a36b6afc0>
2025-03-18 19:18:21,474 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <function resolve_cli_read_timeout at 0x7f8a36b6b1a0>
2025-03-18 19:18:21,475 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <function resolve_cli_connect_timeout at 0x7f8a36b6b100>
2025-03-18 19:18:21,475 - MainThread - botocore.hooks - DEBUG - Event top-level-args-parsed: calling handler <built-in method update of dict object at 0x7f8a36b19900>
2025-03-18 19:18:21,475 - MainThread - botocore.session - DEBUG - Setting config variable for region to 'us-east-1'
2025-03-18 19:18:21,476 - MainThread - awscli.clidriver - DEBUG - CLI version: aws-cli/2.24.21 Python/3.12.9 Linux/6.1.127-135.201.amzn2023.x86_64 exec-env/CloudShell exe/x86_64.amzn.2023
2025-03-18 19:18:21,476 - MainThread - awscli.clidriver - DEBUG - Arguments entered to CLI: ['--region', 'us-east-1', 'logs', 'start-query', '--log-group-name', '/aws/lambda/6896', '--query-string', "filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\\d+) MB\\sMax Memory Used: (?<memoryUsed>\\d+) MB/", '--start-time', '1742205559', '--end-time', '1742248759', '--debug']
2025-03-18 19:18:21,476 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function add_timestamp_parser at 0x7f8a36a48400>
2025-03-18 19:18:21,477 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function register_uri_param_handler at 0x7f8a380a5080>
2025-03-18 19:18:21,477 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function add_binary_formatter at 0x7f8a36ad2480>
2025-03-18 19:18:21,477 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function no_pager_handler at 0x7f8a37bed4e0>
2025-03-18 19:18:21,477 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function inject_assume_role_provider_cache at 0x7f8a36e3fe20>
2025-03-18 19:18:21,480 - MainThread - botocore.utils - DEBUG - IMDS ENDPOINT: http://169.254.169.254/
2025-03-18 19:18:21,482 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function attach_history_handler at 0x7f8a36c99120>
2025-03-18 19:18:21,482 - MainThread - botocore.hooks - DEBUG - Event session-initialized: calling handler <function inject_json_file_cache at 0x7f8a36dfb920>
2025-03-18 19:18:21,499 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/data/logs/2014-03-28/service-2.json
2025-03-18 19:18:21,511 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs: calling handler <function inject_tail_command at 0x7f8a36a5e2a0>
2025-03-18 19:18:21,511 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs: calling handler <function inject_start_live_tail_command at 0x7f8a36a5cae0>
2025-03-18 19:18:21,512 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs: calling handler <function add_waiters at 0x7f8a36a4a2a0>
2025-03-18 19:18:21,532 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs: calling handler <bound method AliasSubCommandInjector.on_building_command_table of <awscli.alias.AliasSubCommandInjector object at 0x7f8a36b02180>>
2025-03-18 19:18:21,533 - MainThread - awscli.clidriver - DEBUG - OrderedDict({'query-language': <awscli.arguments.CLIArgument object at 0x7f8a35c70aa0>, 'log-group-name': <awscli.arguments.CLIArgument object at 0x7f8a35c70a70>, 'log-group-names': <awscli.arguments.ListArgument object at 0x7f8a35c70d40>, 'log-group-identifiers': <awscli.arguments.ListArgument object at 0x7f8a35c70a10>, 'start-time': <awscli.arguments.CLIArgument object at 0x7f8a38374830>, 'end-time': <awscli.arguments.CLIArgument object at 0x7f8a35c70d10>, 'query-string': <awscli.arguments.CLIArgument object at 0x7f8a35c70ce0>, 'limit': <awscli.arguments.CLIArgument object at 0x7f8a35c709e0>})
2025-03-18 19:18:21,534 - MainThread - botocore.hooks - DEBUG - Event building-argument-table.logs.start-query: calling handler <function add_streaming_output_arg at 0x7f8a36a48860>
2025-03-18 19:18:21,534 - MainThread - botocore.hooks - DEBUG - Event building-argument-table.logs.start-query: calling handler <function add_cli_input_json at 0x7f8a36e647c0>
2025-03-18 19:18:21,534 - MainThread - botocore.hooks - DEBUG - Event building-argument-table.logs.start-query: calling handler <function add_cli_input_yaml at 0x7f8a36e64720>
2025-03-18 19:18:21,534 - MainThread - botocore.hooks - DEBUG - Event building-argument-table.logs.start-query: calling handler <function unify_paging_params at 0x7f8a36c5e340>
2025-03-18 19:18:21,551 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/data/logs/2014-03-28/paginators-1.json
2025-03-18 19:18:21,569 - MainThread - botocore.hooks - DEBUG - Event building-argument-table.logs.start-query: calling handler <function add_generate_skeleton at 0x7f8a36b69580>
2025-03-18 19:18:21,569 - MainThread - botocore.hooks - DEBUG - Event before-building-argument-table-parser.logs.start-query: calling handler <bound method OverrideRequiredArgsArgument.override_required_args of <awscli.customizations.cliinput.CliInputJSONArgument object at 0x7f8a35c70c80>>
2025-03-18 19:18:21,569 - MainThread - botocore.hooks - DEBUG - Event before-building-argument-table-parser.logs.start-query: calling handler <bound method OverrideRequiredArgsArgument.override_required_args of <awscli.customizations.cliinput.CliInputYAMLArgument object at 0x7f8a35c70950>>
2025-03-18 19:18:21,570 - MainThread - botocore.hooks - DEBUG - Event before-building-argument-table-parser.logs.start-query: calling handler <bound method GenerateCliSkeletonArgument.override_required_args of <awscli.customizations.generatecliskeleton.GenerateCliSkeletonArgument object at 0x7f8a35c70920>>
2025-03-18 19:18:21,570 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs_start-query: calling handler <function add_waiters at 0x7f8a36a4a2a0>
2025-03-18 19:18:21,570 - MainThread - botocore.hooks - DEBUG - Event building-command-table.logs_start-query: calling handler <bound method AliasSubCommandInjector.on_building_command_table of <awscli.alias.AliasSubCommandInjector object at 0x7f8a36b02180>>
2025-03-18 19:18:21,571 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.query-language: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,572 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.log-group-name: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,572 - MainThread - botocore.hooks - DEBUG - Event process-cli-arg.logs.start-query: calling handler <awscli.argprocess.ParamShorthandParser object at 0x7f8a385a2450>
2025-03-18 19:18:21,572 - MainThread - awscli.arguments - DEBUG - Unpacked value of '/aws/lambda/6896' for parameter "log_group_name": '/aws/lambda/6896'
2025-03-18 19:18:21,572 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.log-group-names: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,572 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.log-group-identifiers: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,572 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.start-time: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,573 - MainThread - botocore.hooks - DEBUG - Event process-cli-arg.logs.start-query: calling handler <awscli.argprocess.ParamShorthandParser object at 0x7f8a385a2450>
2025-03-18 19:18:21,573 - MainThread - awscli.arguments - DEBUG - Unpacked value of 1742205559 for parameter "start_time": 1742205559
2025-03-18 19:18:21,573 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.end-time: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,573 - MainThread - botocore.hooks - DEBUG - Event process-cli-arg.logs.start-query: calling handler <awscli.argprocess.ParamShorthandParser object at 0x7f8a385a2450>
2025-03-18 19:18:21,573 - MainThread - awscli.arguments - DEBUG - Unpacked value of 1742248759 for parameter "end_time": 1742248759
2025-03-18 19:18:21,573 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.query-string: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,573 - MainThread - botocore.hooks - DEBUG - Event process-cli-arg.logs.start-query: calling handler <awscli.argprocess.ParamShorthandParser object at 0x7f8a385a2450>
2025-03-18 19:18:21,573 - MainThread - awscli.arguments - DEBUG - Unpacked value of "filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\\d+) MB\\sMax Memory Used: (?<memoryUsed>\\d+) MB/" for parameter "query_string": "filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\\d+) MB\\sMax Memory Used: (?<memoryUsed>\\d+) MB/"
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.limit: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.cli-input-json: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.cli-input-yaml: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event load-cli-arg.logs.start-query.generate-cli-skeleton: calling handler <awscli.paramfile.URIArgumentHandler object at 0x7f8a35f47080>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event calling-command.logs.start-query: calling handler <bound method CliInputArgument.add_to_call_parameters of <awscli.customizations.cliinput.CliInputJSONArgument object at 0x7f8a35c70c80>>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event calling-command.logs.start-query: calling handler <bound method CliInputArgument.add_to_call_parameters of <awscli.customizations.cliinput.CliInputYAMLArgument object at 0x7f8a35c70950>>
2025-03-18 19:18:21,574 - MainThread - botocore.hooks - DEBUG - Event calling-command.logs.start-query: calling handler <bound method GenerateCliSkeletonArgument.generate_skeleton of <awscli.customizations.generatecliskeleton.GenerateCliSkeletonArgument object at 0x7f8a35c70920>>
2025-03-18 19:18:21,575 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: env
2025-03-18 19:18:21,575 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: assume-role
2025-03-18 19:18:21,575 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: assume-role-with-web-identity
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: sso
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: shared-credentials-file
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: custom-process
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: config-file
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: ec2-credentials-file
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: boto-config
2025-03-18 19:18:21,576 - MainThread - botocore.credentials - DEBUG - Looking for credentials via: container-role
2025-03-18 19:18:21,578 - MainThread - urllib3.connectionpool - DEBUG - Starting new HTTP connection (1): localhost:1338
2025-03-18 19:18:21,580 - MainThread - urllib3.connectionpool - DEBUG - http://localhost:1338 "GET /latest/meta-data/container/security-credentials HTTP/1.1" 200 1184
2025-03-18 19:18:21,583 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/data/endpoints.json
2025-03-18 19:18:21,609 - MainThread - botocore.hooks - DEBUG - Event choose-service-name: calling handler <function handle_service_name_alias at 0x7f8a387277e0>
2025-03-18 19:18:21,624 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/data/logs/2014-03-28/endpoint-rule-set-1.json
2025-03-18 19:18:21,625 - MainThread - botocore.loaders - DEBUG - Loading JSON file: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/data/partitions.json
2025-03-18 19:18:21,628 - MainThread - botocore.hooks - DEBUG - Event creating-client-class.cloudwatch-logs: calling handler <function add_generate_presigned_url at 0x7f8a38694c20>
2025-03-18 19:18:21,628 - MainThread - botocore.configprovider - DEBUG - Looking for endpoint for logs via: environment_service
2025-03-18 19:18:21,628 - MainThread - botocore.configprovider - DEBUG - Looking for endpoint for logs via: environment_global
2025-03-18 19:18:21,628 - MainThread - botocore.configprovider - DEBUG - Looking for endpoint for logs via: config_service
2025-03-18 19:18:21,628 - MainThread - botocore.configprovider - DEBUG - Looking for endpoint for logs via: config_global
2025-03-18 19:18:21,628 - MainThread - botocore.configprovider - DEBUG - No configured endpoint found.
2025-03-18 19:18:21,632 - MainThread - botocore.endpoint - DEBUG - Setting logs timeout as (60, 60)
2025-03-18 19:18:21,633 - MainThread - botocore.hooks - DEBUG - Event provide-client-params.cloudwatch-logs.StartQuery: calling handler <function base64_decode_input_blobs at 0x7f8a36ad2de0>
2025-03-18 19:18:21,634 - MainThread - botocore.hooks - DEBUG - Event before-parameter-build.cloudwatch-logs.StartQuery: calling handler <function generate_idempotent_uuid at 0x7f8a38727d80>
2025-03-18 19:18:21,634 - MainThread - botocore.hooks - DEBUG - Event before-parameter-build.cloudwatch-logs.StartQuery: calling handler <function _handle_request_validation_mode_member at 0x7f8a387527a0>
2025-03-18 19:18:21,634 - MainThread - botocore.regions - DEBUG - Calling endpoint provider with parameters: {'Region': 'us-east-1', 'UseDualStack': False, 'UseFIPS': False}
2025-03-18 19:18:21,635 - MainThread - botocore.regions - DEBUG - Endpoint provider result: https://logs.us-east-1.amazonaws.com
2025-03-18 19:18:21,635 - MainThread - botocore.hooks - DEBUG - Event before-call.cloudwatch-logs.StartQuery: calling handler <function add_query_compatibility_header at 0x7f8a38752700>
2025-03-18 19:18:21,636 - MainThread - botocore.hooks - DEBUG - Event before-call.cloudwatch-logs.StartQuery: calling handler <function inject_api_version_header_if_needed at 0x7f8a387518a0>
2025-03-18 19:18:21,636 - MainThread - botocore.endpoint - DEBUG - Making request for OperationModel(name=StartQuery) with params: {'url_path': '/', 'query_string': '', 'method': 'POST', 'headers': {'X-Amz-Target': 'Logs_20140328.StartQuery', 'Content-Type': 'application/x-amz-json-1.1', 'User-Agent': 'aws-cli/2.24.21 md/awscrt#0.23.8 ua/2.1 os/linux#6.1.127-135.201.amzn2023.x86_64 md/arch#x86_64 lang/python#3.12.9 md/pyimpl#CPython exec-env/CloudShell cfg/retry-mode#standard md/installer#exe md/distrib#amzn.2023 md/prompt#off md/command#logs.start-query'}, 'body': b'{"logGroupName": "/aws/lambda/6896", "startTime": 1742205559, "endTime": 1742248759, "queryString": "filter @type = \'REPORT\' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\\\\d+) MB\\\\sMax Memory Used: (?<memoryUsed>\\\\d+) MB/"}', 'url': 'https://logs.us-east-1.amazonaws.com/', 'context': {'client_region': 'us-east-1', 'client_config': <botocore.config.Config object at 0x7f8a355aeb10>, 'has_streaming_input': False, 'auth_type': None, 'unsigned_payload': None}}
2025-03-18 19:18:21,636 - MainThread - botocore.hooks - DEBUG - Event request-created.cloudwatch-logs.StartQuery: calling handler <bound method RequestSigner.handler of <botocore.signers.RequestSigner object at 0x7f8a355525d0>>
2025-03-18 19:18:21,636 - MainThread - botocore.hooks - DEBUG - Event choose-signer.cloudwatch-logs.StartQuery: calling handler <function set_operation_specific_signer at 0x7f8a38727ba0>
2025-03-18 19:18:21,636 - MainThread - botocore.credentials - DEBUG - Credentials need to be refreshed.
2025-03-18 19:18:21,637 - MainThread - botocore.credentials - DEBUG - Credentials need to be refreshed.
2025-03-18 19:18:21,638 - MainThread - urllib3.connectionpool - DEBUG - http://localhost:1338 "GET /latest/meta-data/container/security-credentials HTTP/1.1" 200 1184
2025-03-18 19:18:21,639 - MainThread - botocore.credentials - DEBUG - Retrieved credentials will expire at: 2025-03-18 19:31:29+00:00
2025-03-18 19:18:21,640 - MainThread - botocore.auth - DEBUG - Calculating signature using v4 auth.
2025-03-18 19:18:21,640 - MainThread - botocore.auth - DEBUG - CanonicalRequest:
POST
/

content-type:application/x-amz-json-1.1
host:logs.us-east-1.amazonaws.com
x-amz-date:20250318T191821Z
x-amz-security-token:xxx
x-amz-target:Logs_20140328.StartQuery
20250318T191821Z
20250318/us-east-1/logs/aws4_request
b73f15ae3585989f78291f81f9ae3038ca27594f2242ff9c3147571df32942ad
2025-03-18 19:18:21,641 - MainThread - botocore.auth - DEBUG - Signature:
xxx
xxxx-03-18 19:18:21,669 - MainThread - botocore.hooks - DEBUG - Event request-created.cloudwatch-logs.StartQuery: calling handler <bound method UserAgentString.rebuild_and_replace_user_agent_handler of <botocore.useragent.UserAgentString object at 0x7f8a355af440>>
2025-03-18 19:18:21,669 - MainThread - botocore.endpoint - DEBUG - Sending http request: <AWSPreparedRequest stream_output=False, method=POST, url=https://logs.us-east-1.amazonaws.com/, headers={'X-Amz-Target': b'Logs_20140328.StartQuery', 'Content-Type': b'application/x-amz-json-1.1', 'User-Agent': b'aws-cli/2.24.21 md/awscrt#0.23.8 ua/2.1 os/linux#6.1.127-135.201.amzn2023.x86_64 md/arch#x86_64 lang/python#3.12.9 md/pyimpl#CPython exec-env/CloudShell cfg/retry-mode#standard md/installer#exe md/distrib#amzn.2023 md/prompt#off md/command#logs.start-query', 'X-Amz-Date': b'20250318T191821Z', 'X-Amz-Security-Token': b'xxxxxxx', 'Authorization': b'AWS4-HMAC-SHA256 Credential=xxxx/20250318/us-east-1/logs/aws4_request, SignedHeaders=content-type;host;x-amz-date;x-amz-security-token;x-amz-target, Signature=xxxxx', 'Content-Length': '237'}>
2025-03-18 19:18:21,669 - MainThread - botocore.hooks - DEBUG - Event request-created.cloudwatch-logs.StartQuery: calling handler <bound method UserAgentString.rebuild_and_replace_user_agent_handler of <botocore.useragent.UserAgentString object at 0x7f8a355af440>>
2025-03-18 19:18:21,669 - MainThread - botocore.endpoint - DEBUG - Sending http request: <AWSPreparedRequest stream_output=False, method=POST, url=https://logs.us-east-1.amazonaws.com/, headers={'X-Amz-Target': b'Logs_20140328.StartQuery', 'Content-Type': b'application/x-amz-json-1.1', 'User-Agent': b'aws-cli/2.24.21 md/awscrt#0.23.8 ua/2.1 os/linux#6.1.127-135.201.amzn2023.x86_64 md/arch#x86_64 lang/python#3.12.9 md/pyimpl#CPython exec-env/CloudShell cfg/retry-mode#standard md/installer#exe md/distrib#amzn.2023 md/prompt#off md/command#logs.start-query', 'X-Amz-Date': b'20250318T191821Z', 'X-Amz-Security-Token': b'xxxxxxx', 'Authorization': b'AWS4-HMAC-SHA256 Credential=xxxxxxx/xxx/us-east-1/logs/aws4_request, SignedHeaders=content-type;host;x-amz-date;x-amz-security-token;x-amz-target, Signature=xxxxx', 'Content-Length': '237'}>2025-03-18 19:18:21,670 - MainThread - botocore.httpsession - DEBUG - Certificate path: /usr/local/aws-cli/v2/2.24.21/dist/awscli/botocore/cacert.pem
2025-03-18 19:18:21,680 - MainThread - urllib3.connectionpool - DEBUG - Starting new HTTPS connection (1): logs.us-east-1.amazonaws.com:443
2025-03-18 19:18:21,756 - MainThread - urllib3.connectionpool - DEBUG - https://logs.us-east-1.amazonaws.com:443 "POST / HTTP/1.1" 200 50
2025-03-18 19:18:21,757 - MainThread - botocore.parsers - DEBUG - Response headers: {'x-amzn-RequestId': '20f83c1e-c1bf-4929-bc6b-7669d46c31eb', 'Content-Type': 'application/x-amz-json-1.1', 'Content-Length': '50', 'Date': 'Tue, 18 Mar 2025 19:18:21 GMT'}
2025-03-18 19:18:21,757 - MainThread - botocore.parsers - DEBUG - Response body:
b'{"queryId":"1bfa8633-e351-4a31-83fc-3709b5ab8680"}'
2025-03-18 19:18:21,758 - MainThread - botocore.hooks - DEBUG - Event needs-retry.cloudwatch-logs.StartQuery: calling handler <bound method RetryHandler.needs_retry of <botocore.retries.standard.RetryHandler object at 0x7f8a355af710>>
2025-03-18 19:18:21,758 - MainThread - botocore.retries.standard - DEBUG - Not retrying request.
2025-03-18 19:18:21,758 - MainThread - botocore.hooks - DEBUG - Event after-call.cloudwatch-logs.StartQuery: calling handler <bound method RetryQuotaChecker.release_retry_quota of <botocore.retries.standard.RetryQuotaChecker object at 0x7f8a355aee40>>
2025-03-18 19:18:21,759 - MainThread - awscli.formatter - DEBUG - RequestId: 20f83c1e-c1bf-4929-bc6b-7669d46c31eb
{
    "queryId": "1bfa8633-e351-4a31-83fc-3709b5ab8680"
}


```

# SDK code snippet 
```js
const queryString = `
  filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>\d+) MB\sMax Memory Used: (?<memoryUsed>\d+) MB/`;
const queryProps = {
  logGroupName: "/aws/lambda/6896",
  startTime: 1742205559, //	Mon Mar 17 2025 02:59:19 GMT-0700 (Pacific Daylight Time)
  endTime: 1742248759, //Mon Mar 17 2025 14:59:19 GMT-0700 (Pacific Daylight Time)
  queryString,
};
logsClient.middlewareStack.add(
  (next) => async (args) => {
    console.log("request : ", args.request);
    const response = await next(args);
    return response;
  },
  { step: "finalizeRequest" }
);
const { queryId } = await logsClient.send(new StartQueryCommand(queryProps));
```

# SDK full log 

```
6928 node index.mjs
request :  HttpRequest {
  method: 'POST',
  hostname: 'logs.us-east-1.amazonaws.com',
  port: undefined,
  query: {},
  headers: {
    'content-type': 'application/x-amz-json-1.1',
    'x-amz-target': 'Logs_20140328.StartQuery',
    'content-length': '228',
    'x-amz-user-agent': 'aws-sdk-js/3.693.0',
    'user-agent': 'aws-sdk-js/3.693.0 ua/2.1 os/darwin#24.1.0 lang/js md/nodejs#20.18.0 api/cloudwatch-logs#3.693.0 m/E,n',
    host: 'logs.us-east-1.amazonaws.com',
    'amz-sdk-invocation-id': '3dd1f066-4af3-4b86-b9e6-770730964fce',
    'amz-sdk-request': 'attempt=1; max=3',
    'x-amz-date': '20250318T201818Z',
    'x-amz-content-sha256': '683c56be3f866b60c097dfdd19a4058f53549672add6b2e51860abb46504112e',
    authorization: 'AWS4-HMAC-SHA256 Credential=xxxx/20250318/us-east-1/logs/aws4_request, SignedHeaders=amz-sdk-invocation-id;amz-sdk-request;content-length;content-type;host;x-amz-content-sha256;x-amz-date;x-amz-target;x-amz-user-agent, Signature=17e8f9b4e394c2c6b3c0d0f64f82be74c6e844db6a6b0de4dd82424d06c68fdd'
  },
  body: `{"logGroupName":"/aws/lambda/6896","startTime":1742205559,"endTime":1742248759,"queryString":"\\n  filter @type = 'REPORT' | parse @message /REPORT (?:.+)Memory Size: (?<memoryLimit>d+) MBsMax Memory Used: (?<memoryUsed>d+) MB/"}`,
  protocol: 'https:',
  path: '/',
  username: undefined,
  password: undefined,
  fragment: undefined
}
request :  HttpRequest {
  method: 'POST',
  hostname: 'logs.us-east-1.amazonaws.com',
  port: undefined,
  query: {},
  headers: {
    'content-type': 'application/x-amz-json-1.1',
    'x-amz-target': 'Logs_20140328.GetQueryResults',
    'content-length': '50',
    'x-amz-user-agent': 'aws-sdk-js/3.693.0',
    'user-agent': 'aws-sdk-js/3.693.0 ua/2.1 os/darwin#24.1.0 lang/js md/nodejs#20.18.0 api/cloudwatch-logs#3.693.0 m/E,n',
    host: 'logs.us-east-1.amazonaws.com',
    'amz-sdk-invocation-id': 'xxx-xxx-xxx-ba8e-xxxx',
    'amz-sdk-request': 'attempt=1; max=3',
    'x-amz-date': '20250318T201819Z',
    'x-amz-content-sha256': '09566c495ae882cf44eed2a98f87d1570a0ecdd3c7253475b854f449cdaff254',
    authorization: 'AWS4-HMAC-SHA256 Credential=xxxxxxx/20250318/us-east-1/logs/aws4_request, SignedHeaders=amz-sdk-invocation-id;amz-sdk-request;content-length;content-type;host;x-amz-content-sha256;x-amz-date;x-amz-target;x-amz-user-agent, Signature=xxxxx'
  },
  body: '{"queryId":"b7472e27-fa25-497b-8c8e-f17a1503f577"}',
  protocol: 'https:',
  path: '/',
  username: undefined,
  password: undefined,
  fragment: undefined
}
request :  HttpRequest {
  method: 'POST',
  hostname: 'logs.us-east-1.amazonaws.com',
  port: undefined,
  query: {},
  headers: {
    'content-type': 'application/x-amz-json-1.1',
    'x-amz-target': 'Logs_20140328.GetQueryResults',
    'content-length': '50',
    'x-amz-user-agent': 'aws-sdk-js/3.693.0',
    'user-agent': 'aws-sdk-js/3.693.0 ua/2.1 os/darwin#24.1.0 lang/js md/nodejs#20.18.0 api/cloudwatch-logs#3.693.0 m/E,n',
    host: 'logs.us-east-1.amazonaws.com',
    'amz-sdk-invocation-id': '77108a26-xxxx-4558-9ab4-xxxx',
    'amz-sdk-request': 'attempt=1; max=3',
    'x-amz-date': '20250318T201820Z',
    'x-amz-content-sha256': 'xxxx',
    authorization: 'AWS4-HMAC-SHA256 Credential=xxx/xxxx/us-east-1/logs/aws4_request, SignedHeaders=amz-sdk-invocation-id;amz-sdk-request;content-length;content-type;host;x-amz-content-sha256;x-amz-date;x-amz-target;x-amz-user-agent, Signature=xxxxxxxx'
  },
  body: '{"queryId":"b7472e27-fa25-497b-8c8e-f17a1503f577"}',
  protocol: 'https:',
  path: '/',
  username: undefined,
  password: undefined,
  fragment: undefined
}
queryID b7472e27-fa25-497b-8c8e-f17a1503f577

```
