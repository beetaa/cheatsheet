.error {
  border: 1px #f00;
  background: #fdd;
}
.error.intrusion {
  font-size: 1.3em;
  font-weight: bold;
}
.intrusion .error {
  display: none;
}
.badError {
  &:extend(.error all);
  border-width: 3px;
}

.foo .bar, .foo .baz {
    display: none;
}

.ext1 .ext2 {
    &:extend(.foo all);
}

.ext3,
.ext4 {
    &:extend(.foo all);
}

div.ext5,
.ext6 > .ext5 {
    width: 100px;
}

.ext7 {
    &:extend(.ext5 all);
}
