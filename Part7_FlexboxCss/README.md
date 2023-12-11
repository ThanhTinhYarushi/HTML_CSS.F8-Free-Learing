# flex item - flex container

## flex container -> thẻ chứa

- main axis: trục chính  
  `Quyết định hướng flex-item được nằm`
  - main start: điểm đầu
  - main end: điểm cuối
- cross axis: trục luôn vuông góc với main axis
  - cross start: điểm đầu
  - cross end: điểm cuối

## flex item -> thẻ con

main size : song song main axis  
cross size: ss cross axis

## Thuộc tính

- display: flex || inline-flex
  `Quyết định xem có sử dụng flexbox hay không`
- flex-direction: row || collum
  `Thay đổi phương hướng main axis`
  `Mặc định -> row`
- flex-wrap: nowrap || wrap || wrap-reverse
  `Mặc định -> nowrap`
  `Xuống dòng`
- flex-basis: length
  `Set kích thước main size`
- justify-content: flex-start || flex-end || center || space-between || space-around
  `Giúp căn phương hướng flex-item cùng hướng main-axis`
- justify-self:
  `nếu xét thằng justify-content cho cha thì không cần sét này cho con nữa`
- align-content:
  `tương tự justify-content nhưng sét theo chiều cross`
- align-self:
  `dùng để xét cho flex-item`
- flex-grow:
  `thay đổi kích thước flex-item`
- flex-shrink:
  `ngược lại flex-grow`
- flex: number  
  `Viết tắt cho các thg flex`
- order: number  
  `...`
- flex-flow
