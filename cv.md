# Kurganov Vladimir

## Contacts

- Phone: +996 555 32-30-76
- E-mail: err0rfrost@gmail.com
- GitHub: [errfrost](https://github.com/errfrost)
- Telegram: [err0rFrost](https://t.me/err0rFrost)

## About Me

An engineer with over 20 years of different experience in software development. After a long time as a software developer
in different companies, I decided to start my own company providing SEO solutions. In 2021 I became interested in crypto
and first started my trading journey, but then became a crypto fan and started learning how blockchain works. Now I
have some Solidity experience and want to participate in developing crypto projects.

## Skills

- HTML, CSS
- React
- NodeJS
- Python
- Solidity
- Git, GitHub

## Code Example

The main part of my Solidity smart contract code. Making trade between 2 different DEXes.
```
function dualDexTrade(address _router1, address _router2, address _token1, address _token2, uint256 _amount) external onlyOwner {
    uint startBalance = IERC20(_token1).balanceOf(address(this));
    uint token2InitialBalance = IERC20(_token2).balanceOf(address(this));
    swap(_router1,_token1, _token2,_amount);
    uint token2Balance = IERC20(_token2).balanceOf(address(this));
    uint tradeableAmount = token2Balance - token2InitialBalance;
    swap(_router2,_token2, _token1,tradeableAmount);
    uint endBalance = IERC20(_token1).balanceOf(address(this));
    require(endBalance > startBalance, "Trade Reverted, No Profit Made");
  }
```

## Experience

- Freelance - Solidity Developer (2021-Present)
- Hive SEO Solution - CEO\Software Developer\SEO Analyst (2010-2022)
- IKEEN - Software Developer (2009–2010)
- Contact Center ClientIterr - Software Developer (2007–2009)
- ISTC - International Sсience and Technology Center - Software Developer (2003–2007)

## Education

- Kyrgyz-Russian Slavic University (2002-2007)
    - Applied Mathematics and Informatics (Master)

## Languages

- English - Intermediate (B1)
- Russian - Native