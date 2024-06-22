# XOREncryptHelper
&emsp;&emsp;用于网易MC存档加密/解密的异或加密算法封装，使用NodeJS实现.
## API
```
/**
 * @param {Buffer} buf - 一个Buffer对象，存储文件二进制数据
 * @returns {Boolean} 如果文件头有加密魔数则返回true
 */
checkFileIsEncrypt(buf): Boolean

/**
 * 加密给定的Buffer对象
 * @param {Buffer} buf - 要加密的Buffer
 * @param {Buffer|Array} key - 密钥，默认值为'88329851'的ASCII编码
 * @returns {Buffer} 加密结果
 */
encryptFile(buf[, key]): Buffer

/**
 * 解密Buffer对象
 * @param {Buffer} buf - 要解密的Buffer
 * @param {Buffer|Array} key - 密钥，默认值为'88329851'
 * @returns {Buffer} 解密结果
 */
decryptFile(buf[, key): Buffer
```
