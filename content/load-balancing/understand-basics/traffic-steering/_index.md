---
pcx_content_type: concept
title: Traffic steering
weight: 4
---

# Traffic steering

When requests come to your load balancer, it distributes them across your pools and endpoints according to three factors:

1.  [Pool and endpoint health](/load-balancing/understand-basics/health-details/): Traffic decisions start with which pools and endpoints are available and should receive traffic.
2.  [Global traffic steering](/load-balancing/understand-basics/traffic-steering/steering-policies/): Policies set on your [load balancer](/load-balancing/load-balancers/) that route traffic to attached and available pools.
3.  [Local traffic steering](/load-balancing/understand-basics/traffic-steering/origin-level-steering/): These are policies set on each [pool](/load-balancing/pools/) that route traffic to available endpoints within the pool.

When a pool or endpoint becomes unhealthy, your load balancer and pools redistribute traffic according to these same policies.
