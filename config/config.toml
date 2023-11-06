[node]
sync_to_genesis = true
idle_tolerance = "20min"
max_attempts = 3
control_logic_default_delay = "1sec"
force_resync = false
shutdown_for_upgrade_timeout = "2min"
upgrade_timeout = "30sec"

[logging]
format = "json"
color = false
abbreviate_modules = false

[consensus]
secret_key_path = "../../keys/secret_key.pem"
max_execution_delay = 3

[network]
public_address = "127.0.0.1:0"
bind_address = "0.0.0.0:22101"
known_addresses = [ "127.0.0.1:22101", "127.0.0.1:22102", "127.0.0.1:22103",]
min_peers_for_initialization = 3
gossip_interval = "30sec"
initial_gossip_delay = "5sec"
max_addr_pending_time = "1min"
handshake_timeout = "20sec"
max_incoming_peer_connections = 3
max_outgoing_byte_rate_non_validators = 0
max_incoming_message_rate_non_validators = 0
max_in_flight_demands = 50
tarpit_version_threshold = "1.2.1"
tarpit_duration = "10min"
tarpit_chance = 0.2
blocklist_retain_duration = "1min"

[rpc_server]
enable_server = true
address = "0.0.0.0:11101"
qps_limit = 100
max_body_bytes = 2621440
cors_origin = ""

[speculative_exec_server]
enable_server = true
address = "0.0.0.0:25101"
qps_limit = 1
max_body_bytes = 2621440
cors_origin = ""

[rest_server]
enable_server = true
address = "0.0.0.0:14101"
qps_limit = 100
cors_origin = ""

[event_stream_server]
enable_server = true
address = "0.0.0.0:18101"
event_stream_buffer_length = 5000
max_concurrent_subscribers = 100
cors_origin = ""

[storage]
path = "../../storage"
max_block_store_size = 19327352832
max_deploy_store_size = 12884901888
max_deploy_metadata_store_size = 12884901888
max_state_store_size = 10737418240
enable_mem_deduplication = true
mem_pool_prune_interval = 4096

[gossip]
infection_target = 3
saturation_limit_percent = 80
finished_entry_duration = "1min"
gossip_request_timeout = "10sec"
get_remainder_timeout = "5sec"
validate_and_store_timeout = "1min"

[block_accumulator]
attempt_execution_threshold = 3
dead_air_interval = "3min"
purge_interval = "5min"

[block_synchronizer]
max_parallel_trie_fetches = 5000
peer_refresh_interval = "90sec"
need_next_interval = "1sec"
disconnect_dishonest_peers_interval = "10sec"
latch_reset_interval = "5sec"
stall_limit = "120sec"

[fetcher]
get_from_peer_timeout = "10sec"

[contract_runtime]
max_global_state_size = 32212254720
max_query_depth = 5
enable_manual_sync = true

[deploy_buffer]
expiry_check_interval = "1min"

[diagnostics_port]
enabled = true
socket_path = "debug.socket"
socket_umask = 63

[upgrade_watcher]
upgrade_check_interval = "30sec"

[consensus.zug]
sync_state_interval = "50ms"
log_participation_interval = "1min"
proposal_timeout = "10sec"
proposal_grace_period = 200
proposal_timeout_inertia = 10
clock_tolerance = "1sec"

[consensus.highway]
pending_vertex_timeout = "1min"
request_state_interval = "20sec"
log_participation_interval = "15sec"
log_synchronizer_interval = "5sec"
log_unit_sizes = false
max_requests_for_vertex = 5
max_request_batch_size = 20

[network.estimator_weights]
consensus = 0
gossip = 0
finality_signatures = 0
deploy_requests = 1
deploy_responses = 1
block_requests = 1
block_responses = 0
trie_requests = 1
trie_responses = 0

[consensus.highway.round_success_meter]
num_rounds_to_consider = 40
num_rounds_slowdown = 10
num_rounds_speedup = 32
acceleration_parameter = 40
acceleration_ftt = [ 1, 100,]
