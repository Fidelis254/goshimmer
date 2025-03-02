# v0.7.5 - 2021-08-09
* Move the scheduler of the congestion control at the end of data flow
* Add new metrics collection
* Add alias initial state validation
* Add creation of new marker sequence after maxVerticesWithoutFutureMarker threshold
* Fix booking of transactions in multiple conflict sets
* Fix manual peering parsing from config.json
* Update JS dependencies
* Update Dockerfile to explicitly expose used ports
* Update docs to docusaurus
* Update snapshot file with DevNet UTXO at 2021-08-09 13:33 UTC
* **Breaking**: bumps network and database versions

# v0.7.4 - 2021-07-08
* Add ParametersDefinition structs in integration test framework
* Add UTXO-DAG interface
* Fix setting correct properties to newly forked branches
* Fix using weak parents for direct approvers when looking for transactions that are approved by a message
* Update entry node from community
* Update docs
* Update snapshot file with DevNet UTXO at 2021-07-08 07:09 UTC
* **Breaking**: bumps network and database versions

# v0.7.3 - 2021-07-01
* Add latest snapshot download from S3
* Add weak tips on local dashboard
* Improve integration test framework
* Add FCoB metrics to remote logger
* Remove tips broadcaster
* Improve APIs
* Fix Sync status
* Fix gossip and requester issues
* Fix Inclusion state inconsistencies
* Fix Prometheus issues when autopeering is not enabled
* Increase maxVerticesWithoutFutureMarker to 3000000
* Update snapshot file with DevNet UTXO at 2021-06-30 21:16 UTC
* Update JS dependencies
* Update hive.go
* **Breaking**: bumps network and database versions

# v0.7.2 - 2021-06-17
* Add local double spend filter in webAPI
* Add SetBranchFinalized to FCoB
* Set message of the weak parents finalized rather than only their payload
* Update snapshot file with DevNet UTXO at 2021-06-17 08:52 UTC
* Update JS dependencies
* **Breaking**: bumps network and database versions

# v0.7.1 - 2021-06-15
* Improve Faucet
* Improve docs
* Improve message requester
* Improve common integration test
* Improve collected Elasticsearch metrics
* Add run callback to database plugin
* Add Client Library Import Check
* Add time range check in wallet lib
* Replace builtin hash map with a sorted set
* Enable Github Actions Caching
* Fix wrong account mention
* Fix gossip neighbor disconnect
* Fix Genesis Loaded Transaction View
* Fix memory leak in pow plugin/pkg
* Fix overlocking and sleeping issues 
* Fix snapshot bug
* Fix typos
* Update Graphana debugging dashboard
* Update snapshot file with DevNet UTXO at 2021-06-15 09:09 UTC
* Update JS dependencies
* **Breaking**: bumps network and database versions

# v0.7.0 - 2021-06-02
* Add client diagnostic API
* Improve docs and tutorials
* Improve congestion control
* Improve dashboard
* Improve Grafana dashboard
* Limit chat fields length
* Fix several bugs
* Reset snapshot file
* Update JS dependencies
* **Breaking**: bumps network and database versions

# v0.6.4 - 2021-05-29
* Add simple chat dApp
* Improve client lib
* Improve manual peering and add tutorial
* Improve docs and tutorials
* Improve congestion control
* Fix mana dashboard deadlock
* Fix several bugs
* Update snapshot file with Pollen UTXO at 2021-05-29 10:22 UTC
* Update JS dependencies
* Update lo latest hive.go
* **Breaking**: bumps network and database versions

# v0.6.3 - 2021-05-25
* Improve congestion control
* Fix builds
* Fix dRNG shutdown deadlock
* Fix panic on booking
* Fix locking management on message factory
* Fix several visualizer bugs
* Update Grafana pie charts
* Update snapshot file with Pollen UTXO at 2021-05-25 16:54 UTC
* **Breaking**: bumps network and database versions

# v0.6.2 - 2021-05-24
* Add Congestion Control
* Add global snapshot
* Add Central Asset Registry to cli-wallet
* Switch to RocksDB instead of BadgerDB
* Enhance manual peering
* Improve gossip
* Improve APIs
* Fix several dashboard bugs
* Update lo latest hive.go
* Update snapshot file 
* **Breaking**: bumps network and database versions

# v0.6.1 - 2021-05-19
* Change Faucet default parameters
* **Breaking**: bumps network and database versions

# v0.6.0 - 2021-05-19
* Add first iteration of the tokenization framework
* Add aMana refresher
* Add CORS to middleware Dashboard server
* Allow specifying parents count when issuing messages 
* Move PoW for Faucet requests to client
* Remove Faucet requests from Node's Dashboard
* Improve cli-wallet
* Improve APIs
* Improve integration tests
* Refactor statement remote logging  
* Display full messageID in explorer feed
* Update JS dependencies
* Update documentation
* **Breaking**: bumps network and database versions

# v0.5.9 - 2021-05-11
* Replace sync beacons with Tangle Time
* Fix approval weight manager persistence
* Fix non positive ticker
* Fix marker issues
* Fix solidification issues
* Fix concurrency-related issues
* Improve FPC metrics logging
* Improve clock synchronization handling
* Improve dRNG plugin
* Improve integration tests
* Update JS dependencies
* Update to latest hive.go
* Update documentation
* **Breaking**: bumps network and database versions

# v0.5.8 - 2021-05-07
* Integrate FPC with the X-Team committee
* Enable finality via approval weight
* Add Tangle Time
* Add sync status monitoring
* Add activity plugin
* Add manual peering support
* Add markers info to message view
* Remove moving average for cMana
* Replace epochs with weight provider using Tangle Time
* Fix marker issues
* Fix sync issues
* Disable past-cone check when booking transactions
* Improve integration tests
* Refactor error handling
* Update snapshot
* Update JS dependencies
* Update to latest hive.go
* Update documentation
* **Breaking**: bumps network and database versions

# v0.5.7 - 2021-04-23
* Add approval weight manager (soft launch)
* Add epochs
* Add debug APIs for epochs
* Update local dashboard to show finalization based on approval weight
* Improve FPC
* Improve markers manager
* Improve integration tests
* Improve payload unmarshaling
* Remove unless-stopped option from Docker default config
* Increase CfgGossipAgeThreshold parameter
* Fix several bugs on hive.go
* Fix mana event storage pruning
* Fix mana leaderboard and explorer live feed scroll view
* Update snapshot with initial mana state
* Update to latest hive.go
* **Breaking**: bumps network and database versions

# v0.5.6 - 2021-04-03
* Fix childBranchType
* Fix FPC empty round increase
* Make reading of FPC statements less strict
* Fix aggregated branch diagnostic API and dashboard page  
* **Breaking**: bumps network and database versions

# v0.5.5 - 2021-04-01
* Integrate Mana with FPC
* Integrate Mana with the Autopeering
* Add several FPC optimizations
* Add dRNG diagnostic API
* Simplify memory usage of dashboard and align to Grafana
* Add a chart for stored, solidifier, scheduler and booker MPS
* Update to latest hive.go
* **Breaking**: bumps network and database versions

# v0.5.4 - 2021-03-29
* Add new diagnostic APIs
* Add new docs sections
* Add branch inclusion state check before issuing new transactions
* Refactor the Faucet plugin
* Optimize transaction's past cone check
* Make issued messages pass through the parser filters
* Fix Faucet time usage
* Fix markers issue
* Fix max inputs count check
* Fix nil pointer in diagnostic API
* Update to latest hive.go 
* Enhance golangci-lint
* **Breaking**: bumps network and database versions

# v0.5.3 - 2021-03-25
* Added new API endpoints
* Added models navigation through the Dashboard Explorer
* Added new diagnostic APIs
* Added new docs sections
* Fix dashboard mana event feed
* Fix markers issue
* Fix UnlockBlocks check
* Fix loading of config parameters
* Fix bug in the Get method of ColoredBalances
* Enhance golangci-lint
* **Breaking**: bumps network and database versions

# v0.5.2 - 2021-03-17
* Fix markers past cone check
* Add more information to explorer and message API
* Restrict Genesis attachment
* Fix parsing of GenesisNode public key
* Display mana histogram in log scale on dashboards
* **Breaking**: bumps network and database versions

# v0.5.1 - 2021-03-15
* Implement FCoB*
* Fix markers persistence bug
* Fix Docker shutdown too early
* Make FCoB fire the MessageOpinionFormed event only if the event for its parents was also fired
* Update JS dependencies
* Refactor parameters in MessageLayer
* Upgrade go to 1.16.2
* Upgrade to latest hive.go
* **Breaking**: bumps network and database versions

# v0.5.0 - 2021-03-11
* Add Mana (currently not used by any of the modules)
* Add Mana APIs
* Add Mana section to the local dashboard
* Add Mana section to the Pollen Analyzer dashboard
* Add Mana section to the Grafana dashboard
* Refactor the Consensus Manager to be independent from the concrete consensus mechanism implemented  
* Improve Tangle visualizer
* Improve documentation
* **Breaking**: bumps network and database versions

# v0.4.1 - 2021-03-02
* Add orphanage analysis tool
* Add documentation web-api
* Simplify past-cone checks
* Improve message findByID API
* Improve value transactionByID API
* Fix saving markers in message metadata
* Fix issue with ReferenceUnlockBlocks
* Fix Faucet address blacklist
* Fix some visualizer glitches
* **Breaking**: bumps network and database versions

# v0.4.0 - 2021-02-26
* Remove the value Tangle
* Add approval switch
* Add Markers integration
* Add new message booker
* Add new ledger state
* Add new opinion former
* Add new Tip manager
* Add new flow unit tests
* Add remote spammer tool
* Add sendTransaction timestamp validity check
* Add clock Since method
* Add docs actions
* Add Tangle width debug tool option
* Update client-lib
* Update wallet
* Update web-API
* Update Grafana dashboard to show MPS for entire data-flow
* Update to latest hive.go
* Refactor integration tests
* Refactor transaction validity check
* Refactor cli-wallet
* Refactor sendTransactionByJson API
* Refactor inclusion state
* Refactor TransactionConfirmed event
* Refactor transaction visualization in the local dashboard
* Refactor scheduler
* Refactor snapshot script
* Fix clock time usage
* Fix wrong handler in the MessageInvalidEvent
* Decrease cache time
* **Breaking**: bumps network and database versions

# v0.3.6 - 2021-02-12
* Finalize Payload layout
* Update dRNG with finalized payload layout
* Add simple scheduler
* Add message approval analysis API
* Add core logic for timestamp voting (still disabled)
* Refactor message parser
* Refactor solidifier
* Refactor Tangle events
* Update entry node URL
* Update gossip to not gossip requested messages
* Introduce invalid message flag
* Merge the new data flow
* Fix visualizer bug
* Update hive.go
* Update JS dependencies
* **Breaking**: bumps network and database versions

# v0.3.5 - 2021-01-13
* Fix consensus statement bug
* Fix deadlock in RandomMap
* Fix several shutdown related issues
* Load old messages in visualizer
* Fix wrong Tips count in visualizer
* Fix dashboard typos
* Improve integration tests
* Improve network delay analysis
* Update hive.go
* Update JS dependencies
* **Breaking**: bumps network and database versions

# v0.3.4 - 2020-12-11
* Revert Pebble to Badger.
* **Breaking**: bumps network and database versions

# v0.3.3 - 2020-12-10
* Fix sync issue.
* Fix pkger issue.
* **Breaking**: bumps network and database versions

# v0.3.2 - 2020-12-09
* Switch from BadgerDB to Pebble.
* Add FPC statements.
* Add clock based time to message metadata.
* Improve dashboard message live feed.
* Improve spammer to evenly distribute issued messages within a minute.
* Fix panic when writing on a closed channel in the dashboard web socket.
* Upgrade Go to 1.15.5
* Upgrade to latest hive.go
* **Breaking**: bumps network and database versions

# v0.3.1 - 2020-11-13
* Refactor message structure according to the new Tangle RFC: 
    * add support for multiple parents
    * update local dashboard
    * new unit tests
    * max payload size changed to 65157 bytes
* Add community-based entry node.
* Add commit tag to version.
* Add package for common sentinel errors.
* Improve dashboard websocket management.
* Integrate NTP-based clock to the network delay app.
* Switch from packer to pkger to pack dashboard.
* Switch from Viper to koanf as core library for configuration.
* Fix Value Tangle tip selection management.
* Fix mps query label in grafana.
* Fix potential race condition within the clock package.
* Upgrade to latest hive.go
* Upgrade NodeJS dependencies of the dashboard.
* **Breaking**: bumps network and database versions

# v0.3.0 - 2020-10-12
* Added multiple dRNG committees support: Pollen, X-Team and Custom.
* Added clock synchronization plugin via NTP.
* Added basic codeQL analysis pipeline for common vulnerability scanning.
* Added basic HTTP authentication.
* Changed payload layout to be more similar to the one specified for Chrysalis phase 2.
* Improved rand-seed tool by writing its output to a file.
* Improved the Docker network by making MongoDB, Grafana and Prometheus optional so that startup/shutdown times are low when not needed.
* Upgraded to the latest hive.go.
* Upgraded NodeJS dependencies of the dashboard.
* Fixed several security issues.
* Refactored the entire code base to make its package structure flat and more consistent with Hornet.
* Moved data structures to hive.go 
* Removed JWT authentication due to security issues of the package dgrijalva/jwt-go
* **Breaking**: bumps network and database versions

# v0.2.4 - 2020-09-03
* Fixes race condition that was preventing the deletion of some entries from missing messages.
* Improves the Tangle-BadgerDB interaction.
* Improved APIs for debug with the addition of the value-tips endpoint.
* Improved autopeering management by adding the ability to specify a given network version.
* Integrates initial support for the dRNG module.
* **Breaking**: bumps network and database versions

# v0.2.3 - 2020-08-11
* Fixes synchronization issue where missing messages were not requested more than once
* Fixes node's dashboard explorer crashing or not properly visualizing the payload of a given message
* Improves Grafana local dashboard:
    * Adds support for the sync-beacon payload type
    * Displaying uptime and nodeID
* Fixed all linter issues to improve code quality
* **Breaking**: bumps network and database versions

# v0.2.2 - 2020-07-27
* Improves message and transaction validation: 
    * Adjust max transaction inputs count;
    * Adds signature validation before issuance; 
    * Enforce max message size in message factory.
* Improves API:
    * Changes granularity of spammer API to accept messages per minute;
    * Adds API middleware and set CORS to allow from every origin;
    * Adds sendTransactionByJSON to allow a client to issue transactions by providing them in a JSON format;
    * Adds tool API endpoint to facilitate debugging of the solidification status;
    * Removes old API documentation;
* Improves synchronization process:
    * Refactors message requester to be more reliable;
    * Improves solidification process;
    * Refactors worker pool management;
    * Replaces bootstrap plugin with the more secure and reliable beacon plugin.
* Improves analysis-server dashboard:
    * Adds the ability to distinguish between different GoShimmer node versions;
    * Refactors the interaction between server side and dashboard;
    * Improves consensus visualization;
    * Improves dashboard tooling.
* Adds a new electron-based wallet.
* Increases max gossip packet size.
* Adds command to the CLI to override database dirty flag.
* Grafana local dashboard
    * Adds messages in database chart (solid, not solid, total)
    * Adds average solidification time chart
    * Adds Message Request Queue Size chart
* **Breaking**: bumps network and database versions

# v0.2.1 - 2020-07-01
* Adds PoW requirement to faucet payloads
* Adds tips broadcaster to ensure that all chains are getting solidified
* Fixes being able to send a double-spend via one node
* **Breaking**: bumps network and database versions

# v0.2.0 - 2020-06-30
* Adds the value transfer dApp:
    * New binary transaction layout
    * UTXO model 
    * Support for transactions with Ed25519 and BLS signatures
    * Parallel reality based ledger state
    * Support for colored tokens
    * Conflict resolution via FPC
    * Applied FCoB rules
* Adds the network delay dApp which is used to gather the avg. network delay occurring in the network
* Adds the faucet dApp giving the ability to request funds for testing via the dashboard or web API
* Adds the DRNG dApp which is used to propagate random numbers produced by a dRand committee (this dApp is inactive)
* Adds the base communication layer
* Adds improved analysis server:
    * Splits it into 3 separate plugins `analysis-client`/`analysis-dashboard`/`analysis-server`
    * Applies heartbeat pattern for robustness on both client and server side
    * Uses TLV denoted messages for communication
    * Complete new dashboard with live visualisations of the network graph and ongoing conflicts
    * Use short node IDs throughout the analysis dashboard
    * Prometheus exporter to expose global network metrics
    * Storage for conflicts inside a MongoDB for further processing
    * Complete rewritten autopeering data retention
* Adds additional HTTP API routes:
    * "healtz" route to query the health of the node (for LBs)
    * Query transaction attachment locations
    * Query transactions by IDs
    * Send transactions
    * Get UTXOs on addresses
    * Query info about the node
    * Issue a faucet funding request
    * Query dRNG committee
    * Query dRNG random number
    * Issue data payloads
* Adds dashboard improvements:
    * Tips chart
    * Communication layer visualizer
    * Address and UTXOs view
    * Message payload view
    * DRNG live feed
    * Faucet page to request funds
    * Support different payload views (data, value, faucet, unknown)
* Adds integration test framework and corresponding tests:
    * Autopeering/Network Split
    * Message propagation 
    * FPC 50/50 network split voting
    * Faucet funding
    * Value transfers
    * Synchronization
* Adds refactored communication layer code
* Adds BLAKE2-based PoW for rate control
* Adds rewritten FPC package
* Adds possibility to change config options with environment variables
* Adds sample Grafana dashboard for local node instances
* Adds snapshot-file import
* Adds "dirty-flag" to the `Database` plugin to check for corrupted databases
* Adds BadgerDB gargbage collection on startup/shutdown and removes periodic GC
* Adds review-dog linter and automatic integration tests execution to continuous integration pipeline
* Adds `Prometheus` exporter plugin with exposure for [following metrics](https://github.com/iotaledger/goshimmer/issues/465)
* Adds `Sync` plugin keeping track of the node's synchronization state
* Adds `Issuer` plugin which takes care of issuing messages (and blocking any issuance when the node is desynced)
* Adds `Profiling` plugin which exposes the `pprof` endpoints and is now configurable
* Adds `Bootstrap` plugin which continuously issues messages to keep the comm. layer graph growing
* Adds proper metrics collection in the `Metrics` plugin
* Adds support for the new HTTP API routes to the Go client library
* Adds `tools/docker-network` to run an isolated GoShimmer network with a chosen amount of nodes. Predefined local and global grafana dashboards are spinned up as well for the network
* Upgrades `hive.go` with various improvements and fixes
* Fixes bind address prints to not be normalized
* Fixes usage of WebSocket message rate limiter
* Fixes disabled/enabled plugins list in info response
* Fixes the `Graceful Shutdown` plugin not showing the actual background workers during shutdown. The node operator is now
able to see pending background workers in the order in which they are supposed to be terminated
* Refactors display of IDs to use Base58 throughout the entire codebase
* Increases network and database versions
* Removes usage of non std `errors` package
* Removes `Graph` plugin
* Renames `SPA` plugin to `Dashboard`
* Makes running GoShimmer with a config file mandatory if not explicitly bypassed

# v0.1.3 - 2020-03-16

* Update SPA plugin's JS dependencies
* Upgrade `github.com/gobuffalo/packr` to v2.8.0
* Resolves a security issue in the packr dependency, which would allow an unauthenticated attacker to read any
 file from the application's filesystem 

# v0.1.2 - 2020-02-24

* Adds `--version` flag to retrieve the GoShimmer version
* Adds the version and commit hash to the remote log logging
* Replaces the autopeering module with the one from hive.go 
* Changed the pprof listen port to `6061` to avoid conflict with Hornet
* Fixes `invalid stored peer` messages
* Fixes masternodes getting removed if they were offline
* Fixes `-c` and `-d` to define config file/dir
* Fixes drop messages about full queues appearing too many times
* Fixes crash due to incopatible transaction size
* Changed the salt lifetime to 2 hours from 30 minutes

# v0.1.1 - 2020-02-07

This release contains a series of fixes:
* Adds logging of the underlying error when a neighbor connection couldn't be established
* Adds the `RemoteLog` plugin (disabled per default) which sends log messages to a centralized logging service
* Removes the status screen plugin in favor of the SPA/dashboard
* Fixes the neighbor send queue being too small causing spam in the log
* Fixes a deadlock which occurred when a neighbor disconnected while at the same time a `request transaction` 
packet was getting processed which was received by the disconnected neighbor
* Fixes memory consumption by disabling BadgerDB's compression
* Fixes analysis server WebSocket replays freezing the backend code
* Fixes sending on the neighbor send queue if the neighbor is disconnected
* Fixes `BufferedConnection`'s read and written bytes to be atomic

# v0.1.0 - 2020-01-31

> Note that this release is a complete breaking change, therefore node operators are instructed to upgrade.

This release mainly integrates the shared codebase between Hornet and GoShimmer called [hive.go](https://github.com/iotaledger/hive.go), 
to foster improvements in both projects simultaneously. Additionally, the autopeering code from [autopeering-sim](https://github.com/iotaledger/autopeering-sim)
has been integrated into the codebase. For developers a Go client library is now available to communicate
with a GoShimmer node in order to issue, get and search zero value transactions and retrieve neighbor information.

A detailed list about the changes in v0.1.0 can be seen under the given [milestone](https://github.com/iotaledger/goshimmer/milestone/1?closed=1).

* Adds config keys to make bind addresses configurable
* Adds a `relay-checker` tool to check transaction propagation
* Adds database versioning
* Adds concrete shutdown order for plugins
* Adds BadgerDB garbage collection routine
* Adds SPA dashboard with TPS and memory chart, neighbors and Tangle explorer (`spa` plugin)
* Adds option to manually define autopeering seed/private keys
* Adds Golang CI and GitHub workflows as part of the continuous integration pipeline
* Adds back off policies when doing network operations
* Adds an open port check which checks whether NATs are configured properly
* Adds `netutil` package
* Adds the glumb visualizer backend as a plugin called `graph` (has to be manually enabled, check the readme)
* Adds rudimentary PoW as a rate control mechanism
* Adds the autopeering code from autopeering-sim
* Adds association between transactions and their address
* Adds the possibility to allow a node to function/start with gossiping disabled
* Adds buffered connections for gossip messages
* Adds an OAS/Swagger specification file for the web API
* Adds web API and refactors endpoints: `broadcastData`, `findTransactionHashes`,
`getNeighbors`, `getTransactionObjectsByHash`, `getTransactionTrytesByHash`, `getTransactionsToApprove`, `spammer`
* Adds a Go client library over the web API
* Adds a complete rewrite of the gossiping layer
* Fixes the autopeering visualizer to conform to the newest autopeering changes.  
  The visualizer can be accessed [here](http://ressims.iota.cafe/).
* Fixes parallel connections by improving the peer selection mechanism
* Fixes that LRU caches are not flushed correctly up on shutdown
* Fixes consistent application naming (removes instances of sole "Shimmer" in favor of "GoShimmer")
* Fixes several analysis server related issues
* Fixes race condition in the PoW code
* Fixes race condition in the `daemon` package
* Fixes several race conditions in the `analysis` package
* Fixes the database not being closed when the node shuts down
* Fixes `webauth` plugin to function properly with the web API
* Fixes solidification related issues
* Fixes several instances of overused goroutine spawning
* Upgrades to [BadgerDB](https://github.com/dgraph-io/badger) v2.0.1
* Upgrades to latest [iota.go](https://github.com/iotaledger/iota.go) library
* Removes sent count from spammed transactions
* Removes usage of `errors.Identifiable` and `github.com/pkg/errors` in favor of standard lib `errors` package
* Use `network`, `parameter`, `events`, `database`, `logger`, `daemon`, `workerpool` and `node` packages from hive.go
* Removes unused plugins (`zmq`, `dashboard`, `ui`)
