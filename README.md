# Zabbix-Template-App-Redis
Zabbix Template App Redis

***

# Steps to follow:
1. Place the script on a REDIS server in the "/etc/zabbix/scripts" folder when you have an Zabbix Agent installed on it.
Also make it executable (`chmod +x`) otherwise it will not work.

2. Edit Zabix hostname in "zbx_redis_stats.py" file at line 13.

3. Import the template called 'zbx-template-redis` into Zabbix Front-End

4. Do not forget to add this to a 'root' crontab:  `* * * * * /etc/zabbix/scripts/zbx_redis_stats.py host_name -p 6379` where "host_name" is the the name of the Redis server.


# Redis Items:

-Redis (arch_bits)

-Redis (aof_enabled)

-Redis (aof_rewrite_in_progress)

-Redis (blocked_clients)

-Redis (connected_clients)

-Redis (client_biggest_input_buf)

-Redis (client_longest_output_list)

-Redis (aof_rewrite_scheduled)

-Redis (connected_slaves)

-Redis (evicted_keys)

-Redis (keyspace_misses)

-Redis (gcc_version)

-Redis (instantaneous_ops_per_sec)

-Redis (keyspace_hits)

-Redis (latest_fork_usec)

-Redis (lru_clock)

-Redis (expired_keys)

-Redis (llenall)

-Redis (loading)

-Redis (mem_fragmentation_ratio)

-Redis (multiplexing_api)

-Redis (redis_git_dirty)

-Redis (pubsub_channels)

-Redis (rdb_bgsave_in_progress)

-Redis (rejected_connections)

-Redis (redis_git_sha1)

-Redis (redis_mode)

-Redis (redis_version)

-Redis (role)

-Redis (rdb_changes_since_last_save)

-Redis (total_commands_processed)

-Redis (used_cpu_user)

-Redis (uptime_in_seconds)

-Redis (used_cpu_sys)

-Redis (used_cpu_user_children)

-Redis (used_memory_rss)

-Redis (total_connections_received)

-Redis (used_cpu_sys_children)

-Redis (used_memory)

-Redis (used_memory_peak)

# Redis Triggers:

-Redis queue length too high

-Redis is down on {HOSTNAME}

# Redis Graphs:

-Redis clients

-Redis ops\total lists

-Redis used_cpu

-Redis used_memory

# For questions or suggestions:
:email:  gpegel@gmail.com
