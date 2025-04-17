## STATS
### Scoreboard
- `P_<stat>`


### Storage
- total `[{id:"",flat:"",additive:"",multiplicative:""}]`
  - id: `<namespace>` (stat)
  - flat: `number`
  - additive: `number`
  - multiplicative: `number`
- modifiers: `[{id:"",total:"",display:"",modifiers:[]}]`
  - __id:__ `<namespace>`
  - __total:__ `[{id:"",flat:"",additive:"",multiplicative:""}]`
    - id: `<namespace>` (stat)
    - flat: `number`
    - additive: `number`
    - multiplicative: `number`
  - __display:__ `{Item:{},name:"",group:"",description:[]}`
    - Item: `{id:"",components:{}}`
      - id: `minecraft:<namespace>`
      - components: `components`
    - name: `<namespace>`
    - group: `<namespace>`
    - description: `SNBT` (text)
  - __modifiers:__ `[{id:"",total:"",display:"",modifiers:[]}]`
