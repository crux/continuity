# Continuity 

Continuity is the run-time container for business logic on top of GOM. Business
logic may be writtin in javascript of ruby. The scripts are connected to GOM
events in a declarative way, the GOM/GNP plumbing is than done by the
container. The scripts are contained in an Actor-Model concurrency model.

Example:

    on_update "/doorbell/ring" do |op, value|
        puts "ding dong!: #{value}"
    end
