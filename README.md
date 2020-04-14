Learning React Router

1. npm install --save react-router react-router-dom
2. Use Route & exact 連接的 URL 必須與 path 完全吻合才行
3. Use Route with Mutil Page，當進到 Page 時會 Reload 整個 Page，Reload Page 會造成之前的state完全不見
   a. 當不要 Reload 整個 page，需使用 React Router Dom 的 Link Component
4. Use withRouter HOC component to get route props
5. Relative Path
   ex: <Link to={props.match.url + '/new'}>
6. Use NavLink to style active link
   a. Use activeClassName to change styel active classname
   b. inline style with activeStyle
7. Route with Parameters
   ex: 
       route  : Route path="/:id" exact component={FullPost} />
       get id : this.props.match.params.id
