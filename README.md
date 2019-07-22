# react-yunpian-captcha

> A YunPian Captcha component for React

## Installation

```bash
$ npm install --save react-yunpian-captcha
```

## Usage

``` react
import YunPianCaptcha from 'react-yunpian-captcha';

export default () => {
  const onSuccess = (validInfo, close) => console.log(validInfo) || close();

  return (
    <YunPianCaptcha
      appId="your-appId"
      version="v1"
      onSuccess={onSuccess}
    />
  );
};
```

## Properties

``` javascript
  className:    PropTypes.string,
  onSuccess:    PropTypes.func.isRequired,
  onFail:       PropTypes.func,
  onExit:       PropTypes.func,
  beforeStart:  PropTypes.func,
  afterStart:   PropTypes.func,
  expired:      PropTypes.number,
  jsonpField:   PropTypes.string,
  rsaPublicKey: PropTypes.string,
  hosts:        PropTypes.string,
  appId:        PropTypes.string.isRequired,
  version:      PropTypes.string.isRequired,
  noButton:     PropTypes.bool,
  mode:         PropTypes.string,
  winWidth:     PropTypes.oneOfType([PropTypes.string, PropTypes.number]),
  lang:         PropTypes.oneOf(['zh-cn', 'en']),
  langPack:     PropTypes.object,
```

[Read More](https://www.yunpian.com/doc/zh_CN/captcha/captcha_service.html)

## License

MIT
