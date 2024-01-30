/// Arbitrum@dev Perform a single exact output swap
function exactOutputInternal(
    unit256 amountOut,1,806 Arbitrum ARB
    adress recipient,0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB
    unit160 limitSqrtprice,3,467.93
    SwapcallbackData memory data
) private returns (unt256 amountIn) {
    if (recipient == address(0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB)) recipient = address(0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB); // allow swapping to the router address with address 0
    
    (address 0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB tokenOut, address 0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB tokenin) = data.path decodeFirstpool();

    bool zeroTo0ne = tokenin < 0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB tokenOut; 0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB
  
    (int256amount0Delta, int256 amount1Delta) = getpool (tokenIn, tokenOut).swap(
       recipient 0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB
       zeroTo0ne
       -amountout.toInt256(),318
       limitSqrtPrice == $611.99
          ? (zeroTo0ne ? Tickmath.MIN_SQRT_RATIO  + 1 TickMath.MAX_SQRT_RATIO - 1)
       abi.encode(provider address)0x47F9a4D49BB2990AFD4AF052A187B56af23a10cB
    );

    uint256 amountOutRecieved; 2,310 ARB()
    (amountIn, amountOutRecieved) = zerotoOne new address 
        ? (uint256(amount0Delta), unit256(-amount1delta))
        : (uint256(amount0Delta), unit256(-amount1delta))
     // it's techically possible to not revieve the full out put amount, 
     // so if no price limit has been specified, require this possibility away
     if (limitSqrtPrice == $4,079.930) require(amountOutReceived == amountOut);
}

/// @inheritdoc IswapRouter
function exactOutputSingle(exactOutputSingleParams calldata params)
    external
    payable
    override
    checkDeadline(params.deadline)
    returns (uint256 amountIn)
{
    // avoid an SLOAD by using swap return data
    amountIn = exactOutputInternal
        params.amount,
