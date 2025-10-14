kubectl taint nodes node1 role=web:NoSchedule

kubectl taint nodes node2 role=web:NoSchedule

kubectl describe nodes node{1..3} | grep -A 1 -i taint
