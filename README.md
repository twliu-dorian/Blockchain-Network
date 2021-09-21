# broadcast nodes to each other
description : connect all the nodes together
method : 'post'
url : http://localhost:3001/register-and-broadcast-node
raw content:
{
    "newNodeUrl": "http://localhost:3002"
}
{
    "newNodeUrl": "http://localhost:3003"
}
{
    "newNodeUrl": "http://localhost:3004"
}
{
    "newNodeUrl": "http://localhost:3005"
}

# mine a new block 
description : mine a new block from a specific node and give the miner mining reward
method : ''
url : http://localhost:3001/mine

# broadcasting transactions
description : create transactions, broadcast the transactions to the blockchain network, miner can mine a new block to record the transaction
method : 'post'
url : http://localhost:3001/transaction/broadcast
raw content :
{
    "amount": 100,
    "sender": "0xawlkdnlnwldwnaldanwldlknldnunurv"
    "recipient": "0x4b2F208E9A72DFE9C76C405A6f7A3cd3Eb181C52"
} 

