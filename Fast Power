class Solution:
    """
    @param a: A 32bit integer
    @param b: A 32bit integer
    @param n: A 32bit integer
    @return: An integer
    """
    def fastPower(self, a, b, n):
        # write your code here
        #运用二进制转换的思想
        #十进制转为二进制时运用短除法取模，一旦取模为1，将结果乘入
        ans = 1 
        while n > 0:
            if n % 2 == 1:
                ans = (ans * a) % b
            a = (a % b) * (a % b)
            n = n // 2
        return ans % b
        #过程中多次取余不影响输出结果，并提高运行速度
