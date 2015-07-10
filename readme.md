# React Tour

React component that help you create nice step-by-step intros.

# Usage

    var ReactTourConfig = [{
      node: React.findDOMNode(this.refs.step1),
      text: 'This is the step 1'
    }, {
      node: React.findDOMNode(this.refs.step2),
      text: 'This is the step 2'
    }, {
      node: React.findDOMNode(this.refs.step3),
      text: 'This is the step 3'
    }];

    // [...]

    <ReactTour config={ReactTourConfig}
      currentStep={<integer>}
      visible={<bool>}
      showDots={<bool>} />

# Props
* `config`: An array that contain the steps of the tour. Each step can have a `node` and `text` properties that contains the dom node to focus and the help text to display.
* `currentStep`: Integer or null.
* `showDots`: Bool. Show progress dots?
* `visible`: Bool. Is the component visible?
