 
    import React from "react";

export default class SubMenuItem extends React.Component {
  render() {
    const list = this.props.submenuList;
    const rows = [];
    if (list !== undefined && list.length !== 0) {
      list.forEach((element) => {
        rows.push(<li key={element.id}>{element.nlskey}</li>);
      });
    }
    return <ul className="submenus"> {rows}</ul>;
  }
}
